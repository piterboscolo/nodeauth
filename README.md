# User Login System using Express and Passport

**Getting Started With MongoDB**

```
C:\mongodb\bin>mongodb --directorydb --dbpath C:\mongo\data\db --logpath C:\mongodb\log\mongodb.log --logappend --install
```

```
net start MongoDB
```
![image](https://user-images.githubusercontent.com/88910148/163369955-f9c89c09-3823-4618-b8c8-aca65036e193.png)


```
db
```

```
use customers
```

```
show dbs
```

```
db.createCollection('customers');
```
![image](https://user-images.githubusercontent.com/88910148/163371478-a1d2f405-32d8-48b4-b780-1eb5b7066cc5.png)

```
use nodeauth
```

```
db.createCollection('users');
```
![image](https://user-images.githubusercontent.com/88910148/163372552-34c6f514-dc8d-4b20-b686-212f6640a10d.png)


```
db.users.insert({name: 'name user' , email: 'email user', username: 'username user' , password: 'ex.: 1234'});
```

***return message***: ![image](https://user-images.githubusercontent.com/88910148/163375577-21c2d66c-7561-44d2-a6fe-1271f2bf813f.png)


***verify user***
```
db.users.find()
```

```
db.users.find().pretty()
```

***insert user***
```
db.users.iunsert({name: 'new name', email:'email@email.com', username: 'new username', password: '12345'});
```

***remove user***
```
db.users.remove({username: 'username'});
```

***App & Middleware Setup***

```
npm install -g express
```
```
npm install
```
```
npm install express-session --save
```

```
npm install
```

***Starnting Server***

```
npm start
```


***Password Hashing with BCrypt***

https://www.npmjs.com/package/bcrypt


Via npm:
```
npm install bcryptjs --save
```

***Passport ogin Authentication***

Simple, unobtrusive authentication for Node.js

Passport is authentication middleware for Node.js. Extremely flexible and modular, Passport can be unobtrusively dropped in to any Express-based web application. A comprehensive set of strategies support authentication using a username and password, Facebook, Twitter, and more.:

https://www.passportjs.org/





