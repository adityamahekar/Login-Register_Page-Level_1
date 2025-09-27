# 🔐 Login & Register Page – Level 1 Authentication

This project is a basic authentication system built with **Node.js**, **Express**, **EJS**, and **PostgreSQL**.  
It demonstrates **Level 1 Authentication** (using email & password without hashing/encryption).

---
## Levels of Encryption:

Level 1: Cipher [Caesor Cipher,Hill Cipher, Playfair Cipher,...]<br>
Level 2: Hashing<br>
Level 3: Salting Rounds + Hashing<br>

---
📂 Project Structure:<br><br>
Authentication+Lv.1<br>
│── css/<br>
│   └── styles.css           Extra CSS file<br>
│<br>
│── public/<br>
│   └── styles.css           Public-facing CSS file<br>
│<br>
│── partials/<br>
│   ├── footer.ejs           Footer partial template<br>
│   └── header.ejs           Header partial template<br>
│<br>
│── views/<br>
│   ├── home.ejs             Home page<br>
│   ├── login.ejs            Login page<br>
│   ├── register.ejs         Register page<br>
│   ├── secrets.ejs          Protected page<br>
│<br>
│── index.js                 Main server file<br>
│── package.json             Dependencies & scripts<br>
│── package-lock.json        Locked dependency versions<br>

---

## 📷 Gallery

| SignUp Page | Login Page|
|----|------------|
| ![lgl1](./imgg/lgl1.png) | ![lgl4](./imgg/lgl4.png)|

| Register Page| Secret Page|
|----------------|-----------------|
|![lgl2](./imgg/lgl2.png)   | ![lgl3](./imgg/lgl3.png) |

| DataBase | 
|-------------------|
| ![lgl5](./imgg/lgl5.png) |

---

## ⚙️ Setup Instructions

 1️⃣ Create Table in PostgreSQL(users):
 <br><br>
as given in the query.sql
 <br>
 
2️⃣ Install Dependencies:
```bash
npm i
npm i pg express ejs body-parser
```

3️⃣ Database Connection (index.js)
```bash
const app = express()
const db = new pg.Client({
  user: "postgres",
  host: "localhost",
  database: "XXXXX",    // <-- your database name
  password: "XXXXX",    // <-- your password
  port: XXXX,           // <-- your port name, by default for pg 5432
});
```
4️⃣ Run Server:
```bash
node index.js
```
---
👉 [Open App on Localhost](http://localhost:3000)
