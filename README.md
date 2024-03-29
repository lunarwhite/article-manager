# article-manager
A simple web app with microservice written in Golang and Gin, to manager articles.
```
.
├── LICENSE
├── README.md
├── common_test.go
├── go.mod
├── go.sum
├── handlers.article.go
├── handlers.article_test.go
├── main.go
├── models.article.go
├── models.article_test.go
├── routes.go
└── templates
    ├── article.html
    ├── footer.html
    ├── header.html
    ├── index.html
    └── menu.html
```

## setup envs
- golang

## features
- Let users register with a username and a password (non-logged in users only)
- Let users login with a username and a password (non-logged in users only)
- Let users log out (logged in users only)
- Let users create new articles (logged in users only)
- Display the list of all articles on the home page (for all users)
- Display a single article on its own page (for all users)

## how it works
- control flow
  ```
  Request -> Route Parser -> [Optional Middleware] -> Route Handler -> [Optional Middleware] -> Response
  ```
- functionalities offered by Gin
  - Routing — to handle various URLs
  - Custom rendering — to handle the response format
  - Middleware — to implement authentication

## run & deploy
- run
  ```shell
  go run mian.go
  ```
- visit `localhost:8080`

## reference
- [Building Go Web Applications and Microservices Using Gin](https://semaphoreci.com/community/tutorials/building-go-web-applications-and-microservices-using-gin)
