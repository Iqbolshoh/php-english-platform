# 🔠 PHP English Platform

This is an **English learning platform** designed to help users improve their **vocabulary, sentence structure, and reading skills**. Users can **register, add vocabulary, create sentences, translate texts**, and complete exercises to enhance learning.  

---

## ✨ **Features**  

✅ **📝 User Registration & Login** – Sign up, log in, and manage your profile.  
✅ **📖 Vocabulary** – Add words with **translations & definitions**.  
✅ **🗣 Sentences** – Create sentences using **your added words** with translations.  
✅ **📜 Texts** – Upload and translate texts for **reading practice**.  
✅ **🧩 Exercises**  
   - 🎯 **Vocabulary Test** – Choose the correct meaning from **4 options**.  
   - 🔠 **Sentence Test** – Arrange **scrambled sentences** into a correct form.  
✅ **📥 Download PDFs** – Save **vocabulary, sentences, and texts** as PDFs.  
✅ **🔍 Search** – Find words, sentences, and texts easily.  
✅ **⭐ Favorites** – Save your **favorite words, sentences, and texts**.  

---

## 🏠 **Pages Overview**  

### 🌍 **Home Page**  
![🏠 Home Page](./src/images/home.png)  
👤 **User Login:** `iqbolshoh`  
👤 **Guest Login:** `user` 
🔐 **Password:** `IQBOLSHOH` 

📌 The **home page** welcomes users and provides navigation to all sections.  

---

### 📚 **Dictionary Page**  
![📖 Dictionary](./src/images/dictionary.png)  

📌 **Add & View Vocabulary**  
📌 Store **words, translations, and definitions**  

---

### 📝 **Sentences Page**  
![🗣 Sentences](./src/images/sentences.png)  

📌 **Create & View Sentences**  
📌 Use words from the **dictionary** and add translations  

---

### 📜 **Texts Page**  
![📄 Texts](./src/images/texts.png)  

📌 **Upload & Read Texts**  
📌 Add **translations for practice**  

---

### 🎯 **Exercises Page**  
![🧩 Exercises](./src/images/exercise.png)  

📌 **Interactive tests** for vocabulary and sentences  
📌 Improve **English skills with quizzes**  

---

### ⚙ **Settings Page**  
![🔧 Settings](./src/images/settings.png)  

📌 **Manage account settings** and preferences  

---

## 🚀 **Installation**  

1️⃣ **Clone the repository:**  

```bash
git clone https://github.com/Iqbolshoh/php-english-platform.git
```

2️⃣ **Navigate to the project directory:**  

```bash
cd php-english-platform
```

3️⃣ **Install dependencies (if applicable):**  

```bash
npm install
```

4️⃣ **Set up the database:**  

- Create a database **named `english`**  
- Import the provided **`database.sql`** file:  

```sql
CREATE DATABASE english;

USE english;

CREATE TABLE users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    fullname VARCHAR(255) NULL,
    email VARCHAR(255) NOT NULL UNIQUE,
    username VARCHAR(150) NOT NULL UNIQUE,
    password VARCHAR(255) NOT NULL,
    profile_image VARCHAR(255) DEFAULT 'default.png',
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
```

5️⃣ **Configure `config.php` with database credentials:**  

```php
public function __construct()
    {
        $servername = "localhost";
        $username = "root";
        $password = "";
        $dbname = "english";

        $this->conn = new mysqli($servername, $username, $password, $dbname);

        if ($this->conn->connect_error) {
            die("Connection failed: " . $this->conn->connect_error);
        }
    }
```

6️⃣ **Start the server:**  

- If using **XAMPP/MAMP**, place the project folder in `htdocs`.  
- Open **`http://localhost/php-english-platform`** in your browser.  

---

## 🏆 **Usage Guide**  

1️⃣ **Register/Login** to access features  
2️⃣ **Add words, sentences, and texts** for practice  
3️⃣ **Take exercises** to improve your skills  
4️⃣ **Download PDFs** of your learning materials  

🚀 **Start learning English the smart way!** 🎓📚

---

## 🖥 Technologies Used
![HTML](https://img.shields.io/badge/HTML-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-%23563D7C.svg?style=for-the-badge&logo=bootstrap&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-%23F7DF1C.svg?style=for-the-badge&logo=javascript&logoColor=black)
![jQuery](https://img.shields.io/badge/jQuery-%230e76a8.svg?style=for-the-badge&logo=jquery&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-%23777BB4.svg?style=for-the-badge&logo=php&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-%234479A1.svg?style=for-the-badge&logo=mysql&logoColor=white)

## 📜 License
This project is open-source and available under the **MIT License**.

## 🤝 Contributing  
🎯 Contributions are welcome! If you have suggestions or want to enhance the project, feel free to fork the repository and submit a pull request.

## 📬 Connect with Me  
💬 I love meeting new people and discussing tech, business, and creative ideas. Let’s connect! You can reach me on these platforms:

<div align="center">
  <table>
    <tr>
      <td>
        <a href="https://iqbolshoh.uz" target="_blank">
          <img src="https://img.icons8.com/color/48/domain.png" 
               height="40" width="40" alt="Website" title="Website" />
        </a>
      </td>
      <td>
        <a href="mailto:iilhomjonov777@gmail.com" target="_blank">
          <img src="https://github.com/gayanvoice/github-active-users-monitor/blob/master/public/images/icons/gmail.svg"
               height="40" width="40" alt="Email" title="Email" />
        </a>
      </td>
      <td>
        <a href="https://github.com/iqbolshoh" target="_blank">
          <img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/github.svg"
               height="40" width="40" alt="GitHub" title="GitHub" />
        </a>
      </td>
      <td>
        <a href="https://www.linkedin.com/in/iqbolshoh/" target="_blank">
          <img src="https://github.com/gayanvoice/github-active-users-monitor/blob/master/public/images/icons/linkedin.svg"
               height="40" width="40" alt="LinkedIn" title="LinkedIn" />
        </a>
      </td>
      <td>
        <a href="https://t.me/iqbolshoh_777" target="_blank">
          <img src="https://github.com/gayanvoice/github-active-users-monitor/blob/master/public/images/icons/telegram.svg"
               height="40" width="40" alt="Telegram" title="Telegram" />
        </a>
      </td>
      <td>
        <a href="https://wa.me/998997799333" target="_blank">
          <img src="https://github.com/gayanvoice/github-active-users-monitor/blob/master/public/images/icons/whatsapp.svg"
               height="40" width="40" alt="WhatsApp" title="WhatsApp" />
        </a>
      </td>
      <td>
        <a href="https://instagram.com/iqbolshoh_777" target="_blank">
          <img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/instagram.svg"
               height="40" width="40" alt="Instagram" title="Instagram" />
        </a>
      </td>
      <td>
        <a href="https://x.com/iqbolshoh_777" target="_blank">
          <img src="https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white"
               height="40" width="40" alt="X" title="X (Twitter)" />
        </a>
      </td>
      <td>
        <a href="https://www.youtube.com/@Iqbolshoh_777" target="_blank">
          <img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/youtube.svg"
               height="40" width="40" alt="YouTube" title="YouTube" />
        </a>
      </td>
    </tr>
  </table>
</div>
