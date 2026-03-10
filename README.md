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

---

# Пример структуры проекта

```id="st3l4q"
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

```bash id="g0y6nb"
git init
git add .
git commit -m "Initial project structure"
```

Создание рабочей ветки:

```bash id="0z5t8r"
git checkout -b feature/my-feature
```

Коммиты:

```bash id="r6a3o6"
git add .
git commit -m "Add feature"
```

Отправка изменений:

```bash id="l3p3cs"
git push -u origin feature/my-feature
```

После этого создайте **Pull Request** и выполните **merge** в `main`.

---

# Теги релиза

Создание релизов:

```bash id="n2o6az"
git tag -a v1.0 -m "First release"
git push origin v1.0
```

```bash id="u6d2lu"
git tag -a v1.1 -m "Improvements"
git push origin v1.1
```

---

# Python окружение

Создание виртуального окружения:

```bash id="e6j6df"
python -m venv venv
```

Установка пакета:

```bash id="pfv63t"
pip install requests
```

Сохранение зависимостей:

```bash id="zpxy4f"
pip freeze > requirements.txt
```

---

# Примечание

Вы можете использовать **любой сервис для размещения Git-репозиториев**, например:

* GitHub
* GitLab
* Bitbucket
* https://gitflic.ru/

Главное требование — чтобы проект поддерживал **Git, ветки, Pull Request (или Merge Request) и теги**.

---

# Что нужно сдать

1. Ссылка на **репозиторий проекта**
2. Вывод команды:

```bash id="p6w0yz"
git log --oneline --graph --all
```
