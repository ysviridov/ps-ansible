# Прохождение курса Ansible от Purple School

Работа в WSL:

Чтобы потом работать:

## Вариант 1. Поставить Ansible через apt (системный пакет)

```sudo apt update
sudo apt install ansible
````

Плюсы:
- Просто
- Интеграция с системой

Минусы:
- Версия Ansible может быть не самая свежая.

Проверка:
ansible --version


---

## Вариант 2. Использовать venv (рекомендуется для разработки)

1. Убедись, что есть модуль venv:
```sudo apt update
sudo apt install python3-venv
```

2. Создай виртуальное окружение в своем проекте:
```cd ~/VSCode/GitHub/ps-ansible
python3 -m venv .venv
```

3. Активируй окружение:
```
source .venv/bin/activate
```

В начале строки терминала появится (.venv).

4. Теперь можно ставить ansible через pip (это уже не системный Python):
```
pip install --upgrade pip
pip install ansible
```

5. Проверка:
```
ansible --version
which ansible
```

## Работа

```bash
cd ~/VSCode/GitHub/ps-ansible
source .venv/bin/activate
# работаем с ansible...
deactivate  # когда закончишь
```

