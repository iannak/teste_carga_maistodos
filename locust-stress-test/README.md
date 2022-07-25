# Locust Stress tests 

## Introduction

[Locust](https://github.com/locustio/locust) is an open source load testing tool. From the original repo:
> Locust is an easy-to-use, distributed, user load testing tool. It is intended for load-testing web sites (or other systems) and figuring out how many concurrent users a system can handle. 

## Prerequisites

- Make sure you have python 3.7+ installed
- Install [poetry](https://python-poetry.org/) to manage dependencies.

## Installation

- Install the project with: `pip install poetry && poetry install`

#### Web interface:
```
poetry run locust --host=http://localhost:8000
```


#### Command line

```
poetry run locust --host=http://localhost:8000 --users 100 --spawn-rate 2 --headless
```