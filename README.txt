Quiz Hub — статический одностраничный сайт тестов (nginx-ready)

Структура:
- index.html       — SPA, отображает тесты из /tests/index.json
- /tests/
  - index.json     — манифест тестов
  - naruto.json    — тест «Кто ты из Наруто?»
  - example.json   — пример теста

Деплой:
1) Скопируйте содержимое в /var/www/quiz-hub
2) Убедитесь, что nginx конфиг указывает root /var/www/quiz-hub;
3) Перезапустите nginx: sudo nginx -t && sudo systemctl reload nginx

Формат теста: JSON, содержит title, description, characters и questions.
