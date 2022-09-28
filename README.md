# Postman-task
Регистрация https://blog.kata.academy/api/users
POST
{
  "user": {
    "username": "IrinaKukina",
    "email": "avira@mail.ru",
    "password": "12345678"
  }
}
Response
{
    "user": {
        "username": "irinakukina",
        "email": "avira@mail.ru",
        "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYzMzJjYWRjM2NmNzA1MWIwMDgyYThiMSIsInVzZXJuYW1lIjoiaXJpbmFrdWtpbmEiLCJleHAiOjE2Njk0NTcxMTYsImlhdCI6MTY2NDI3MzExNn0.E1vx0ZF5_7J7Kkj7704X5FpNqmnAZVM74-VjVIR9UJM"
    }
}

Авторизация https://blog.kata.academy/api/users/login
POST
{
  "user": {
    "email": "avira@mail.ru",
    "password": "12345678"
  }
}
Response
{
    "user": {
        "username": "irinakukina",
        "email": "avira@mail.ru",
        "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYzMzJjYWRjM2NmNzA1MWIwMDgyYThiMSIsInVzZXJuYW1lIjoiaXJpbmFrdWtpbmEiLCJleHAiOjE2Njk0NTc0NDAsImlhdCI6MTY2NDI3MzQ0MH0.QJlkIkv5IHLJ7nrF1Dh96AvZyMuuwHOiCynfcWB6L3o"
    }
}
Получаем данные
GET
//пустое тело. копируем полученный токен во вкладку Authorization -> Bearer Token
Response
{
    "user": {
        "username": "irinakukina",
        "email": "avira@mail.ru",
        "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYzMzJjYWRjM2NmNzA1MWIwMDgyYThiMSIsInVzZXJuYW1lIjoiaXJpbmFrdWtpbmEiLCJleHAiOjE2Njk0NTgwNTEsImlhdCI6MTY2NDI3NDA1MX0.RElflRlu5wLNymm_xtH889rnjf8P8NYS_oYLH9IBLTY"
    }
}
