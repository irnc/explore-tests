## Introduction

* we have MongoDB database with real data extracted from legacy data source;
* this database is about to change rapidly during the course of the project;
* we have mongoose models serving as data access layer on this database;
* mongoose models serve express routes;
* express routes are utilized by adapters from Ember application;
* Ember application has a lot of business logic rules and calculations based on data.

## Mongoose Models

Mongoose models can contain business logic, but in our case, all business logic was programmed in Ember application, leaving only data access responsibility to mongoose models.

There is no point in unit testing these mongoose models, as they does not contain business logic. Data access functionality can not be tested without MongoDB database, as there is no point in mocking query processor and aggregation pipelines.

So we goes to test integration between Mongoose models and MongoDB server. The question is: should we test on empty database inserting fake data, or should we test on a copy of real database.

## Express Routes

## Ember Application Adapters

## Ember Components
