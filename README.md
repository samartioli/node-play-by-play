

##Pre-Requisites

1. Install Mongo

  `brew install mongodb`

2. Install Redis

  `brew install redis`

3. Install Nodemon and Forever

  `npm i -g nodemon forever`

4. Create the data folder

  `mkdir /data/db`

5. Give permissions to the data folder

  `sudo chown john /data/db`

##Run Mongo, Redis, and the Servers

1. Open a terminal and run `redis-server`

2. Open another terminal tab and run `mongod`

3. Open another terminal and run

  ```
  forever start cat_server.js
  forever start dog_server.js
  nodemon pet_server.js
  ```

