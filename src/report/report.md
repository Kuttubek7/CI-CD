Part 1. Настройка gitlab-runner

1. Установка Ubuntu Server 20.04 LTS
2. Установка gitlab-runner
![install_gitlab_runner](part1/install_gitlab-runner.png)

3. Регистрация пользователя в gitlab-runner
![register_user_gitlab_runner](part1/register_gitlab-runner.png)


Part 2. Сборка

1. Этап CI для сборки проекта
![](part2/build.png)

2. Результат сборки проекта
![](part2/result_build.png)

Part 3. Тест кодстайла

1. Cкрипт который будет проверять кодстайл проекта
![](part3/style_test_bash.png)

2. Этап CI в файле .gitlab-ci.yml
![](part3/style.png)

3. Кодстайл успешно прошел
![](part3/style_test_success.png)

4. Кодстайл успешно провален
![](part3/style_test_fail.png)

Part 4. Интеграционные тесты

1. Этап CI для теста
![](part4/integration_test.png)

2. Выполненный результат
![](part4/integration_test_result.png)

Part 5. Этап деплоя

1. Этап CD
![](part5/deploy.png)

2. Скрипт для переноса испольняемого файла на второй сервер
![](part5/deploy_bash.png)

3. Результаты деплоя
![](part5/deploy_result.png)
![](part5/deploy_result_2server.png)

Part 6. Дополнительно. Уведомления

1. Для того чтобы он отправлял нам уведомление после каждого выполненного CICD немного изменил файл .gitlab-ci.yml
![](part6/notification.png)

2. Написал bash скрипт для проверки результатов выполнения кода
![](part6/notification_bash.png)

3. Результат уведомлений в телеграмм боте


![](part6/result_notification.jpg)
