---
layout: default
title: Create a Typer Application
---

# Create a Typer Application

## Goal

Create a modern command-line application using Typer.

Typer makes it easy to build CLIs with:

- type hints
- automatic help text
- argument parsing
- command groups
- autocompletion support

It is one of the simplest ways to build Python command-line tools.

---

## Ingredients

Install Typer:

```bash
pip install typer
````

***

## Recipe

Create a file named:

```text
cli.py
```

Add:

```python
import typer

app = typer.Typer()


@app.command()
def hello(name: str):
    print(f"Hello {name}!")


if __name__ == "__main__":
    app()
```

Run:

```bash
python cli.py hello Jonas
```

Output:

```text
Hello Jonas!
```

***

## How It Works

A Typer application starts by creating an application object:

```python
app = typer.Typer()
```

Commands are registered using:

```python
@app.command()
```

Function parameters automatically become command-line arguments.

For example:

```python
def hello(name: str):
    ...
```

becomes:

```bash
python cli.py hello Jonas
```

without needing to manually parse arguments.

***

## Automatic Help

Typer automatically provides help output.

Run:

```bash
python cli.py --help
```

Example:

```text
Usage: cli.py [OPTIONS] COMMAND [ARGS]...

Commands:
  hello
```

Command help:

```bash
python cli.py hello --help
```

This is one of Typer's biggest advantages compared to manually parsing arguments.

***

## Why Use Typer?

Typer provides:

* simple syntax
* excellent developer experience
* automatic help generation
* strong type hint integration
* support for larger applications

Many modern Python CLI projects use Typer because it scales from small scripts to larger tools.

***

## Project Structure

Small projects often start with:

```text
project/
│
├── cli.py
├── README.md
└── pyproject.toml
```

As projects grow, a common structure becomes:

```text
project/
│
├── src/
│   └── project/
│       ├── cli.py
│       ├── commands/
│       └── services/
│
├── tests/
├── README.md
└── pyproject.toml
```

***

## Variations

### Positional Arguments

```python
@app.command()
def greet(name: str):
    print(f"Hello {name}")
```

Usage:

```bash
python cli.py greet Jonas
```

***

### Options

```python
@app.command()
def greet(
    name: str,
    uppercase: bool = False
):
    if uppercase:
        print(name.upper())
    else:
        print(name)
```

Usage:

```bash
python cli.py greet Jonas --uppercase
```

***

### Multiple Commands

```python
import typer

app = typer.Typer()


@app.command()
def hello():
    print("Hello")


@app.command()
def goodbye():
    print("Goodbye")


if __name__ == "__main__":
    app()
```

Usage:

```bash
python cli.py hello
python cli.py goodbye
```

***

## When Would I Use This?

Typer is a good choice when building:

* developer tools
* automation scripts
* internal utilities
* AI applications
* personal productivity tools
* data processing pipelines

Many projects start as a simple Typer application and later evolve into larger tools.

***

## Related Recipes

* Add Command Arguments
* Add Command Options
* Interactive User Prompts
* Rich Terminal Output
* Configuration Files
* Package a CLI Tool

***

## Official Documentation

* <https://typer.tiangolo.com/>

