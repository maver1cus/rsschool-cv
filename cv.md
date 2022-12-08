# Sergey Petrov

Located in **Moscow, Russia**

## Contacts
- Telegram:  [@mavericusdev](https://t.me/mavericusdev)
- Email: [mavericusdev@gmail.com](mailto:mavericusdev@gmail.com)
- LinkedIn: [linkedin.com/in/mavericus](https://www.linkedin.com/in/mavericus/)
- GitHub: [https://github.com/maver1cus](https://github.com/maver1cus/)
- VKontakte: [vk.com/mavericusdev](https://vk.com/mavericusdev/)

## Summary

    I work as a frontend developer in a small company. I am responsible for the work of the company's websites.

# Skills

- HTML (Pug, Nunjucks)
- CSS  (SCSS, SASS, LESS)
- JavaScript (ES5, ES6)
- ReactJS (NextJS)
- Node (Express, NestJS)
- GIT

- Programming languages
  - JavaScript
  - PHP
  - HTML
  - CSS
- Frameworks
  - ReactJS
  - NextJS
  - NestJS
  - Express
  - Laravel
- Databases
  - MySQL
  - PostgreSQL
  - MongoDB
  - SQLite
- Other
  - Git
  - GitHub
  - Postman
  - Webpack, Gulp

## Code examples

- [питомник-туй.москва](http://xn----otbafdkhgh5agm.xn--80adxhks/)
- [Game Derby](https://github.com/maver1cus/game-derby)
- [GTD planer](https://github.com/maver1cus/planner)

```JavaScript
const jwt = require('jsonwebtoken')
const status = require('http-status')
const secret = process.env.SECRET_KEY;
module.exports = function (req, res, next) {
  if (req.method === "OPTIONS") {
    next()
  }
  try {
    const token = req.headers.authorization.split(' ')[1] || null;
    if (!token) {
      return res.status(status.FORBIDDEN).json({message: "Пользователь не авторизован"})
    }
    const decodedData = jwt.verify(token, secret)
    req.user = decodedData
    next()
  } catch (e) {
    return res.status(status.FORBIDDEN).json({message: "Пользователь не авторизован"})
  }
};
```

## Education

  - 1998-2002 Alexandrovsky Industrial Humanitarian College
  
    Operator of computing equipment and automated control systems
  
  - 2020 RS School
  
    NodeJS 2020 Q3

## English leve
My level is A1. I am constantly improving my English. I read books, watch you-tube channels and use applications
