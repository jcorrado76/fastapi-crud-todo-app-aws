# crud_todo_list_app_fastapi_aws

## Introduction

This project is an implementation of the CRUD todo-list app from the tutorial YouTube video [here](https://www.youtube.com/watch?v=iLt00bqp6is&list=WL&index=8).

The upstream repo for the code from the tutorial can be found [here](git@github.com:pixegami/todo-list-api.git).


CRUD:

* create
* read
* update
* delete

## Tech Stack

* AWS API Gateway
* AWS Lambda
* AWS DynamoDB
* AWS CDK
* Python FastAPI

## Data Model

A single table (`tasks`) with schema:

* task_id - integer
* user_id - string
* created_time - timestamp
* content - string
* is_done - bool

## Public API

* GET /
* PUT /create-task
* GET /get-task/{task_id}
* GET /list-tasks/{user_id}
* PUT /update-task
* DELETE /delete-task/{task_id}

## TODOs

* use FERN to specify API