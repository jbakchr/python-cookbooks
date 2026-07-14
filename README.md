# python-cookbooks

A collection of practical Python cookbooks and implementation recipes.

The goal of this project is not to teach Python from scratch or document every Python feature.

The goal is to provide reusable guides for building real-world Python projects and solving common implementation problems.

***

## Why This Project Exists

I often find myself thinking:

> "I know I've done this before."

Maybe I need to:

* build a CLI application
* call an API
* load configuration files
* add structured logging
* package a Python project
* create a FastAPI service

The solution usually exists somewhere in an old repository.

This project gathers those solutions into organized cookbooks that are easier to find, understand, and reuse.

***

## What Is a Cookbook?

A cookbook is a collection of practical recipes focused on accomplishing a specific goal.

For example:

```text
CLI Applications
├── Create a Typer Application
├── Add Configuration Files
├── Use Rich for Output
└── Package a CLI Tool

Web APIs
├── Make HTTP Requests
├── Handle Authentication
├── Retry Failed Requests
└── Paginate API Results

AI Applications
├── Call Ollama
├── Manage Prompt Templates
├── Structured LLM Output
└── Store Conversation History
```

Each recipe focuses on solving a real problem and explaining when and why a particular approach is useful.

***

## Guiding Principles

### Practical First

Recipes should focus on real-world implementation tasks.

### Small and Focused

Each recipe should solve a single problem.

### Modern Python

Prefer modern Python approaches whenever reasonable.

### Standard Library First

Use the Python standard library when it provides a good solution.

### Explain the Why

Recipes should do more than provide code.

They should explain:

* why the solution works
* when it is useful
* when alternative approaches may be better

### Reusable

The content should be easy to apply to future projects.

***

## Planned Cookbooks

### CLI Applications

Recipes for building command-line applications using tools such as Typer and Rich.

### Files and Configuration

Recipes for JSON, YAML, TOML, environment variables, and configuration management.

### Web APIs

Recipes for making HTTP requests, authentication, retries, and pagination.

### FastAPI

Recipes for building APIs with FastAPI.

### Testing

Recipes using pytest and related testing tools.

### Logging

Recipes for application logging and debugging.

### Packaging and Distribution

Recipes for packaging Python applications and publishing packages.

### AI Applications

Recipes for building applications that use LLMs and local models.

### Automation and Scripting

Recipes for common automation and workflow tasks.

***

## Recipe Structure

Most recipes will follow a consistent structure:

### Goal

What are we trying to accomplish?

### Ingredients

Libraries, tools, or dependencies required.

### Recipe

Step-by-step implementation.

### Variations

Alternative approaches and trade-offs.

### When Would I Use This?

Practical scenarios where the solution is useful.

### Related Recipes

Connections to other recipes and cookbooks.

***

## Relationship to easier-python-docs

This project complements, but does not replace, easier-python-docs.

### easier-python-docs

Focused on questions like:

```text
How do I read a JSON file?

How do I join paths?

How do I remove duplicates from a list?
```

Its goal is to help discover the right Python solution.

### python-cookbooks

Focused on questions like:

```text
How do I build a CLI tool?

How do I structure a FastAPI project?

How do I add structured logging?

How do I package a Python application?
```

Its goal is to help implement real-world solutions.

***

## Current Status

🚧 Early development

The initial focus is:

* establishing cookbook categories
* creating foundational recipes
* documenting patterns used across personal projects
* building a practical Python implementation knowledge base

***

## License

MIT License
