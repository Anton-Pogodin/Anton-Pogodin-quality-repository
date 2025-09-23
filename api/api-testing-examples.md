# Примеры тестирования API (CRUD)

**Файл примера:** [API_Testing.pdf](../screenshots/9.%20API_Testing.pdf)

## 1. GET-запрос - получение данных пользователя
GET /api/users/123
Authorization: Bearer token123

## 2. POST-запрос - создание нового пользователя
POST /api/users
Content-Type: application/json

{
  "name": "Test User",
  "email": "test@example.com"
}

## 3. PUT-запрос - обновление данных
PUT /api/users/123
Content-Type: application/json

{
  "name": "Updated Name"
}

## 4. DELETE-запрос - удаление пользователя
DELETE /api/users/123
Authorization: Bearer token123