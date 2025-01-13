## GIT

**Git** — это распределенная система управления версиями. Она позволяет разработчикам отслеживать изменения в коде, совместно работать над проектами и управлять историей разработки.

### Основные возможности:
* Отслеживание изменений в файлах.
* Возможность возвращаться к предыдущим версиям.
* Работа в команде через репозитории.

### Основные понятия в Git:
* Репозиторий — хранилище кода и истории изменений.
* Коммит — сохранение изменений.
* Ветка — отдельная линия разработки.
* Слияние (merge) — объединение веток.
* Удаленный репозиторий — репозиторий на сервере (например, GitHub, GitLab).

## Установка Git:
1. Загрузите и установите Git с git-scm.com.
2. Проверьте установку:
```bash
git --version
```

##  Базовые команды Git:

1. Настройка имени и email:
```bash
git config --global user.name "Ваше Имя"
git config --global user.email "ваш_email@example.com"
```

2. Инициализация репозитория:
```bash
git init
```

3. Добавление файлов в индекс (staging area):
```bash
git add <имя_файла>
git add . # Добавить все файлы
```

4. Создание коммита:
```bash
git commit -m "Описание изменений"
```

5. Просмотр состояния репозитория:
```bash
git status
```

6. Просмотр истории изменений:
```bash
git log
```

7. Создание ветки:
```bash
git branch <имя_ветки>
```

8. Переключение между ветками:
```bash
git checkout <имя_ветки>
```

9. Слияние веток:
```bash
git merge <имя_ветки>
```

10. Клонирование удаленного репозитория:
```bash
git clone <url_репозитория>
```

11. Отправка изменений в удаленный репозиторий:
```bash
git push origin <ветка>
```

12. Получение изменений из удаленного репозитория:
```bash
git pull
```

## Пример работы с Git:
1. Создание нового репозитория:
   ```bash
   mkdir my_project
   cd my_project
   git init
   echo "Hello, Git!" > README.md
   git add README.md
   git commit -m "Initial commit"
   ```

2. Работа с ветками:
   ```bash
   git branch feature_branch
   git checkout feature_branch
   echo "Feature code" > feature.txt
   git add feature.txt
   git commit -m "Added feature"
   git checkout main
   git merge feature_branch
   ```

3. Работа с удаленным репозиторием:
   ```bash
   git remote add origin https://github.com/username/my_project.git
   git push -u origin main 
   ```

опять накосячил