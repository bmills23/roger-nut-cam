# README

This is the roger nut cam.

## To run the server

### Prerequisites

1. mysql (mysql-server on ubuntu)
2. nodejs 
	* using version 16.15.1
	* `sudo npm install -g n`
	* `sudo n 16.15.1`

### 1st time setup


setup a mysql user named `ship` and give the user some priveleges
```
cd FrontEnd
sudo mysql -u root -p < add_server_user.sql
```

setup DB and create tables
```
mysql -u ship -p < create_db.sql
```

### start node server

```
npm run devStart
```