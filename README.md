# Spring2023
The project will parse xml and create tables on the database based on the xml file.
The languages are used for the project implementation:Python, Node.js, Html,CSS,XML,SQL(Query Language),MariaDB
The below dependencies and modules are used for the project implementation:,Morgan,Mysql,Mustache,session,http,path,express,support,handlebars,
express- handlebars,nodemon, npm init is required for node js
The below libraries used for the project implementation:os,mysql.connector,error,xml.etree.ElementTree
The data set downloaded are xml files : https://www.nsf.gov/awardsearch/download.jsp
The project will create dabase connectivity and then parse though each parent and child element of xml file and as per syntax create tables.
The second part os the project will then again connect to database to get information from web, that is run though localhost port.
The project is very simple and easy to undersatnd with one pager code in py file and with proper saperation of view, mdules and main code in node js.
The project can be find here in github and also can be find in docker (just pull the image) docker push salukumari/nsf:v2


```
python data/sql/prepare.py
python train.py config/train_sql.py --device=cpu --compile=False --eval_iters=20 --log_interval=1 --block_size=64 --batch_size=12 --n_layer=4 --n_head=4 --n_embd=128 --max_iters=2000 --lr_decay_iters=2000 --dropout=0.0
python sample.py --out_dir=text-to-sql --device=cpu --start="create table"
```
