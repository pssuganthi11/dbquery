# 📚 DB QUERY

## MongoDB CRUD Queries

Basic **CRUD operations** using **MongoDB** for a **Book Shop database**.

---

## 🗄 Creating Database

```javascript
use("book_shop")
```

<img src="./Assets/createdb.png" width="500"/>

---

##  Insert One Data

```javascript
db.books.insertOne({
  id: 1,
  book_name: "The Alchemist",
  book_author: "Paulo Coelho",
  book_published_date: "1988-04-15",
  book_price: 499
})
```

<img src="./Assets/insertone.png" width="500"/>

---

##  Insert Many Data

```javascript
db.books.insertMany([
{
  id: 2,
  book_name: "Atomic Habits",
  book_author: "James Clear",
  book_published_date: "2018-10-16",
  book_price: 699
},
{
  id: 3,
  book_name: "Rich Dad Poor Dad",
  book_author: "Robert Kiyosaki",
  book_published_date: "1997-04-01",
  book_price: 550
}
])
```

<img src="./Assets/insertmany.png" width="500"/>

---

##  Update One Data

```javascript
db.books.updateOne(
 { id: 1 },
 { $set: { book_price: 600 } }
)
```

<img src="./Assets/updateone.png" width="500"/>

---

##  Update Many Data

```javascript
db.books.updateMany(
 { book_price: { $lt: 600 } },
 { $set: { book_price: 600 } }
)
```

<img src="./Assets/updatemany.png" width="500"/>

---

##  Find One Data

```javascript
db.books.findOne({ id: 1 })
```

<img src="./Assets/findone.png" width="500"/>

---

##  Find All Data

```javascript
db.books.find()
```

<img src="./Assets/findall.png" width="500"/>

---

##  Delete One Data

```javascript
db.books.deleteOne({ id: 2 })
```

<img src="./Assets/deleteone.png" width="500"/>

---

##  Delete Many Data

```javascript
db.books.deleteMany({ book_price: { $gt: 500 } })
```

<img src="./Assets/deletemany.png" width="500"/>

---




## 🛠 Tools Used

- MongoDB  
- MongoDB Compass  
- GitHub  

---

## 👩‍💻 Author

**Suganthi**
