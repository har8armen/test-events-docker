# Docker Compose - React, Laravel, MySQL

To start please create some folder for this project

    git clone git@github.com:har8armen/test-events-docker.git events
    cd events

### Frontend

    git clone git@github.com:har8armen/test-events-frontend.git frontend

And then follow the instructions on [Github Frontend](https://github.com/har8armen/test-events-frontend) Readme file for frontend.

### Backend

    git clone git@github.com:har8armen/test-events-backend.git backend

And then follow the instructions on [Github Backend](https://github.com/har8armen/test-events-backend) Readme file for backend.

Change .env keys as there

    DB_HOST=db
    DB_PORT=3306
    DB_DATABASE=inforepository
    DB_USERNAME=root
    DB_PASSWORD=root

### Docker configuration setup

If you have no installed Docker, install it using [Docker official site](https://www.docker.com/products/docker-desktop).
Then run this command on root folder (events folder)

    docker-compose up

After all you can go to http://localhost:3000 website and if you set up everything okay, you'll see events table with ability to sort them by Date.

Your project structure must be like this:

    .
    ├── ...
    ├── events                    # root folder
    │   ├── backend/              # backend laravel app
    │   ├── frontend/             # frontend react-js app
    │   └── docker-compose.yml    # definitions for docker
    └── ...
