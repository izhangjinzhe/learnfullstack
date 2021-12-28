##### 使用/登录

- `mongo`
- `show dbs`
- `db`
- `use db`
- `db.auth([username],[password])`

##### CURD

[https://mongodb.net.cn/manual/crud/](https://mongodb.net.cn/manual/crud/)

- `db.collection.insertOne(data)`
- `db.collection.insertMany([...data])`
- `db.collection.find(!filter)`
- `db.collection.updateOne(filter,data)`
- `db.collection.updateMany(filter,data)`
- `db.collection.deletOne(filter)`
- `db.collection.deleteMany(filter)`

###### Mongoose

mongoose(引入mongoose)>schema(创建scema)>model(生成model)>instance(创建实例)
