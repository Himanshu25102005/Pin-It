# 📌 Pin-It

Welcome to **Pint-It** — a full-stack image-sharing web app inspired by Pinterest! Built using **Node.js**, **Express**, **MongoDB**, **Mongoose**, and **EJS**, this project demonstrates essential features like user authentication, profile management, file uploads, and post feeds.

---



## ✨ Features

- 👤 **User Registration & Login** (via `passport-local-mongoose`)
- 🖼️ **Upload & Share Pins** (with `multer`)
- 🔒 **Secure Authentication & Sessions**
- 📄 **Profile Page** with image, username, bio
- 📷 **Feed Section** displaying all posts
- ❤️ **Like Posts** (optional feature added)
- 📦 **MongoDB** schema-based models using `mongoose`

---

## 🧠 Tech Stack

| Tech        | Use                     |
|-------------|--------------------------|
| Node.js     | Backend runtime          |
| Express     | Backend framework        |
| MongoDB     | Database                 |
| Mongoose    | ODM for MongoDB          |
| EJS         | Templating engine        |
| Multer      | File/image upload handling |
| Passport.js | Authentication           |
| Tailwind CSS| Frontend utility styles  |

---

## 🗂️ Folder Structure

```
📦Pinterest_Clone/
 ┣ 📁routes/
 ┃ ┣ 📄index.js
 ┃ ┗ 📄users.js
 ┣ 📁models/
 ┃ ┣ 📄user.js
 ┃ ┗ 📄post.js
 ┣ 📁public/
 ┃ ┣ 📁images/uploads/
 ┃ ┗ 📁stylesheets/
 ┃ ┃ ┗ 📄style.css
 ┣ 📁views/
 ┃ ┣ 📄register.ejs
 ┃ ┣ 📄login.ejs
 ┃ ┣ 📄profile.ejs
 ┃ ┣ 📄feed.ejs
 ┃ ┗ 📄partials/
 ┃   ┣ 📄header.ejs
 ┃   ┗ 📄footer.ejs
 ┣ 📄README.md
 ┣ 📄app.js
 ┣ 📄package.json
 ┗ 📄.gitignore
```

---

## 📸 Screenshots


![Home](screenshots/ss1.png)

### 🧑‍💼 Profile Page
![Profile](screenshots/ss2.png)

### ➕ Create Post Page
![Create Post](screenshots/ss3.png)

---

## 🛠️ Installation

```bash
# Clone the repo
git clone https://github.com/Himanshu25102005/Pinterest_Clone.git

# Navigate to the project folder
cd Pinterest_Clone

# Install dependencies
npm install

# Start the server
npm start
```

---

## 🧪 MongoDB Setup

1. Ensure MongoDB is running on your local machine.
2. The database is configured as:
   ```
   mongodb://127.0.0.1:27017/Naya_Pin_DB
   ```

---

## 📄 Models Overview

### 👤 User Model

```js
{
  username: String,
  name: String,
  email: String,
  password: String,
  profileImage: String,
  contact: Number,
  posts: [ObjectId (ref to Post)]
}
```

### 🖼️ Post Model

```js
{
  user: ObjectId (ref to User),
  title: String,
  description: String,
  image: String (filename),
  likes: [ObjectId] (ref to Users who liked)
}
```

---

## 🧠 Concepts Demonstrated

- RESTful Routing
- Middleware (`isLoggedIn`)
- MVC structure
- EJS templating
- Static asset handling
- MongoDB document relationships with `populate`

---

## 🙋‍♂️ Author

**Himanshu Dusane**  
📧 himanshudusane25@gmail.com  
🌐 [GitHub](https://github.com/Himanshu25102005)

---

## ⭐ Show Some Love

If you liked this project, consider giving it a ⭐ on GitHub!

---

## 📃 License

MIT © Himanshu Dusane
