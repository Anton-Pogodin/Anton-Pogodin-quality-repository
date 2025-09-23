# Базовые SQL запросы для тестирования

**Файл примеров:** [SQL_Queries.pdf](../screenshots/8.%20SQL_Queries.pdf)

-- 1. Проверка существования пользователя
SELECT * FROM users WHERE email = 'test@example.com';

-- 2. Проверка количества заказов
SELECT COUNT(*) FROM orders WHERE status = 'completed';

-- 3. Проверка данных за период
SELECT * FROM logs WHERE created_at BETWEEN '2024-01-01' AND '2024-01-31';

-- 4. Проверка связи между таблицами
SELECT u.name, o.order_date 
FROM users u 
JOIN orders o ON u.id = o.user_id;