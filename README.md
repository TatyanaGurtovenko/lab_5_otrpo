# lab_5_otrpo

Python-скрипт для сбора данных из VK и сохранения их в графовую базу данных Neo4j.

## Запуск

1. Клонируйте репозиторий:
    ```bash
    git clone https://github.com/TatyanaGurtovenko/lab_5_otrpo
    cd lab_5_otrpo
    ```


2. Установите необходимые зависимости:
    ```bash
    pip install -r requirements.txt
    ```


3. Создайте файл .env в корневой папке проекта и добавьте в него следующие переменные:
    ```bash
      NEO4J_URL=bolt://localhost:7687
      NEO4J_USER=neo4j
      NEO4J_PASSWORD=your_neo4j_password
      AUTH_TOKEN=your_secret_token
    ```

4. Запустите приложение с помощью Uvicorn:
    ```bash
       uvicorn main:app
    ```
    
5. Для запуска тестов используйте pytest.

 ```bash
   pytest test.py
 ```
