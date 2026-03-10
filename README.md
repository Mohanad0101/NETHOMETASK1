# Домашнее задание — Командный Git проект

**Срок:** до следующей лекции
**Команда:** 2–4 человека
**Платформа:** любой Git-хостинг (GitHub, GitLab или аналог)

---

# Задача

Создайте простое **Python-приложение** в команде и используйте основные возможности **Git**: ветки, коммиты, Pull Request, слияния и теги.

---

# Требования

Проект должен содержать:

* минимум **3 Python файла**

  * `main.py`
  * `utils.py`
  * `config.py`
* минимум **2 feature-ветки**
* минимум **10 коммитов** с понятными сообщениями
* минимум **1 merge**
* настроенный `.gitignore`
* **виртуальное окружение (`venv`)**
* **один внешний пакет** и файл `requirements.txt`
* **теги релизов:** `v1.0` и `v1.1`
* минимум **1 Pull Request**

Дополнительное требование:

* **каждый участник команды должен сделать как минимум 2 коммита** в репозиторий.

---

# Пример структуры проекта

```id="b4gy0f"
my_project/
│
├── main.py
├── utils.py
├── config.py
├── requirements.txt
├── .gitignore
└── README.md
```

---

# Основные команды Git

Инициализация проекта:

```bash id="vqgfdm"
git init
git add .
git commit -m "Initial project structure"
```

Создание рабочей ветки:

```bash id="gqsn3n"
git checkout -b feature/my-feature
```

Коммиты:

```bash id="8xap5q"
git add .
git commit -m "Add feature"
```

Отправка изменений:

```bash id="o3a4zy"
git push -u origin feature/my-feature
```

После этого создайте **Pull Request** и выполните **merge** в `main`.

---

# Теги релиза

Создание релизов:

```bash id="fxye33"
git tag -a v1.0 -m "First release"
git push origin v1.0
```

```bash id="yo9ztn"
git tag -a v1.1 -m "Improvements"
git push origin v1.1
```

---

# Python окружение

Создание виртуального окружения:

```bash id="lbe80j"
python -m venv venv
```

Установка пакета:

```bash id="1n6o45"
pip install requests
```

Сохранение зависимостей:

```bash id="8f9j1f"
pip freeze > requirements.txt
```

---

# Примечание

Вы можете использовать **любой сервис для размещения Git-репозиториев**, например:

* GitHub
* GitLab
* Bitbucket
* https://gitflic.ru/

Главное требование — чтобы платформа поддерживала **Git, ветки, Pull Request (или Merge Request) и теги**.

---

# Что нужно сдать

1. Ссылка на **репозиторий проекта**
2. Вывод команды:

```bash id="dmux1l"
git log --oneline --graph --all
```

---

# Презентация проекта

На следующем лабораторном занятии каждая команда должна **кратко представить свой проект**:

* показать репозиторий
* объяснить структуру проекта
* продемонстрировать работу программы
* рассказать, как использовались ветки и Pull Request
* кратко описать вклад каждого участника команды
