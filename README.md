# WMS SSI DB

## Database provisioning for WMS SSI API in development environment

### Goals

Provide up and running instances of MySQL and Redis to be used in the development of [WMS SSI API](https://github.com/SourceCheckOrg/wms-ssi-api)


#### Note

The Docker Compose configuration is intended to be used only in development environments where exposing default network ports brings no security risks. 


### Prerequisites

You need to have Docker (https://docs.docker.com/engine/install/) and Docker Compose https://docs.docker.com/compose/install/) installed in your machine before using this configuration.


### How to use this repo


1. Clone the repository

```
git clone https://github.com/SourceCheckOrg/wms-ssi-db.git
```

2. Create a file named `.env` on the ROOT directory based on the file `.env.sample`

3. Adjust the database name and root password for the MySQL database

4. Run the following Docker Compose command: 

```
docker-compose up -d 
```

The data is stored in the `data` directory  