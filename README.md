# jobSearchIK

This is an automation framework with a job service running which takes filter selected by student as input and returns the list of jobs selected. The job's selected is a union of all the filters to make it more selective. The logic can be changed to intersection as well.
The automation suite works on top of that. It includes unit tests, contract tests and functional tests in TDD format.
It is also integrated with CI and tests run on any commit to main branch
Ci link: https://app.circleci.com/pipelines/github/bhuvanwy/jobSearchIK/

# dependencies: 
- pytest~=6.2.3
- virtualenv
- flask
- requests~=2.25.1
- jsonschema~=3.2.0

# Steps: 
- Install from requirements.txt
- run flask app using flask run
- run oytest for the tests

# Structure

## data
It contains any redundant data that can be shared across classes like base url for service. This also includes pre seeded data for running the suite.

## utility
It has all the utilities like building requests, geting json from file.

## helper
It has pages corresponding to each endpoint in a service

## tests
It has tests that consumes from helper and run using pytest


## Runs on CI:
<img width="1762" alt="Screenshot 2022-01-22 at 11 23 33 PM" src="https://user-images.githubusercontent.com/13623482/150650198-3c410861-77d4-4a58-86ef-46f070946484.png">
<img width="1764" alt="Screenshot 2022-01-22 at 11 23 43 PM" src="https://user-images.githubusercontent.com/13623482/150650204-f866c8d0-8df5-44cc-a72c-dfcb8a834e5b.png">

