# Welcome to the Anythink Market repo

To start the app use Docker. It will start both frontend and backend, including all the relevant dependencies, and the db.

Please find more info about each part in the relevant Readme file ([frontend](frontend/readme.md) and [backend](backend/README.md)).

## Development

When implementing a new feature or fixing a bug, please create a new pull request against `main` from a feature/bug branch and add `@vanessa-cooper` as reviewer.

## First setup

1. Install Docker

    Go to <https://docs.docker.com/get-docker/> to get docker installed. Once complete, you can verify everything works as expected by running the following commands

    ```shell
    docker -v
    # Docker version 20.10.14, build a224086
    docker-compose -v
    # docker-compose version 1.29.2, build 5becea4c
    ```

1. Use `docker-compose` to stand up the containers

    Run the following command to start the containers

    ```shell
    docker-compose up
    ```

    There will be a lot of logs that get printed out after that, but it should eventually stop scrolling. At that point you can verify the backend and frontend are running.

1. Verification

    In your browser, go to <http://localhost:3000/api/ping> and you should get a message indicating the backend is up.

    In your browser, go to <http://localhost:3001/register> and register for an account. This verifies your frontend is running.

