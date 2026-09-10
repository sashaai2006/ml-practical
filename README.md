# Практикум по машинному обучению

> Репозиторий с домашними заданиями и конспектами по курсу **«Практикум по машинному обучению»**  

## Студент

**Муляр Саша** — Б24-527, НИЯУ МИФИ, ПИ ИИ  
mail: <sasiijob@gmail.com>  
TG: [@sshmulyar](https://t.me/sshmulyar)

Проект использует [uv](https://docs.astral.sh/uv/) для управления зависимостями.

## Структура репозитория

* **`/class-work`** — задания, выполненные на семинарах.
* **`/home-work`** — домашние задания.

## Установка uv

**macOS / Linux:**

```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

> Если `curl` не установлен
>
> ```bash
> sudo apt update && sudo apt install curl
> ```

**Windows (PowerShell):**

```powershell
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
```

> После установки перезапусти терминал, чтобы `uv` стал доступен в PATH.

## Установка проекта

Команды ниже одинаковые для Windows, macOS и Linux:

```bash
git clone https://github.com/sasii/ml-practical.git
cd ml-practical
uv sync
```

## Использование

Все команды запускаются через `uv run` и работают одинаково на любой системе:

```bash
# Jupyter-ноутбуки
uv run jupyter notebook

# Консольный скрипт проекта
uv run ml-practical

# Произвольный Python-скрипт
uv run python src/ml_practical/__init__.py
```
