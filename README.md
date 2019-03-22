# MySQL test_db
docker image for MySQL test_db.

test_db from [https://github.com/datacharmer/test_db](https://github.com/datacharmer/test_db)

## Set up
```
docker run -d \
	--name mysql-test-db \
	-p 3306:3306 \
	-e MYSQL_ROOT_PASSWORD=your_password \
	-v $PWD/data:/var/lib/mysql \
	theoklein/mysql-test-db
```