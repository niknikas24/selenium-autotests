## Установка и запуск

- **0.** Предварительно необходимо скачать с официального сайта (https://git-scm.com/download/win) и установить на компьютере "Git Bash".

  Для корректной работы желательно произвести предварительную настройку `Git Bash`, согласно руководству с оф. сайта (https://git-scm.com/book/ru/v2/Введение-Первоначальная-настройка-Git).

- **1.** Необходимо скачать с официального сайта (https://www.python.org/) и установить на компьютер `Python` (версию не ниже 3.13.4)

- **2.** Необходимо скачать `Docker Desktop` на Windows (https://docs.docker.com/desktop/setup/install/windows-install/) с официального сайта и установить.

- **3.** Загрузить драйвер `ChromeDriver` (https://googlechromelabs.github.io/chrome-for-testing/#stable) для браузера `Google Chrome` с официального сайта.


- **4.** Клонируйте репозиторий:
   Запустите "Командную строку".
   
    - 4.1. Введите в строке команду:

    `git clone https://github.com/niknikas24/selenium-autotests.git`


- **5.** Предварительная настройка:

    - 5.1. Открыть `Командную строку` и ввести (для Windows):

    `pip install --upgrade pip`
	
    `pip install -r requirements.txt`

    `pip install requests`

    `pip install pytest`  

    `pip install pluggy` 


- **6.** Запуск «OpenCart»:

    - 6.1. Запустить `Docker Desktop`

    - 6.2. Открыть `Windows PowerShell` ИЛИ `Командная строку` и ввести: 

    `cd C:\Users\current_user_name\selenium-autotests` 

    `docker-compose up -d` ИЛИ `docker compose up -d`

  «OpenCart» будет доступен на: `http://localhost:8081`

- **7.** Остановка:

    - 7.1. В `Windows PowerShell` ИЛИ `Командная строку` ввести:
  
    `docker-compose down` ИЛИ `docker compose down`

  `Примечание: вместо "current_user_name" - нужно вписать имя текущего пользователя компьютера!`


- **8.** Теперь можно перейти к самим тестам. Запустить `Docker Desktop`:

    - 8.1. Запустить `Командная строку` ИЛИ `Windows PowerShell` и ввести:

    `cd C:\Users\current_user_name\selenium-autotests\tests`

    `pytest`

  `Примечание: вместо "current_user_name" - нужно вписать имя текущего пользователя компьютера!` 
