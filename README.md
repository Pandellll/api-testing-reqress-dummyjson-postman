# API Testing with Postman - Beginner Portfolio

This repository contains a **collection of API tests** using Postman as part of learning the basics of **Manual QA testing**.

---

## 🛠 Tools Used

- [Postman](https://www.postman.com/) - for creating adn executing request
- [Reqres API](https://reqres.in) - for simple test endpoints (GET and POST only)
- [DummyJSON API](https://dummyjson.com/) - for full data manipulation testing
- Manual assertions and test scripting with postman

---

## 📁 Collection Structure

This collection includes **two public APIs** used for testing:

### 1. Reqres API
- **Base URL:** 'https://reqres.in/'
- **Used for:** basic **GET** and **POST** requests

### 2. DummyJSON API
- **Base URL:** 'https://dummyjson.com/'
- **Used for:** **data update and deletion** (POST,PUT, PATCH, DELETE (GET already used on Reqress) and test automation

---

## 🧪 Reqress API Tests

### 🔹 GET - List Users
- **Endpoint** 'https://reqress.in/api/users?page=2'
- **Tests:**
  - Status is 200
  - Validate response contains user list
  - Check user fields like 'email', 'first_name', etc.
 
  ---

### 🔹 POST - Create User
- **Endpoint:** 'https://reqress.in/api/users'
- **Request body:**
  '''json
{
  "name": "Pandellll",
  "job": QAEngineer"
}
  - **Test:**
   - Status is 201
   - Response includes the same 'name' and 'job' sent in body

 ---

## 🧪 DummyJSON API Tests

### 🔹POST - Create User
- **Endpoint:** 'https://dummyjson.com/users/add
- **Request Body:**
'''json
{
  "firstname": "Pandelllll",
  "lastname": "QAEngineer"
}
- **Test:**
  - Status is 200
  - Response includes the same 'firstname' and 'lastname'

---

### 🔹 PUT - Update User
- **Endpoint:** 'https://dummyjson.com/users/1
- **Request Body:**
'''json
{
  "firstname": "PandelllllUpadte",
  "lastname": "QAEngineerUpdated"
}
- **Test:** Status is 200
- Validate update 'firstname' and 'lastname'

---

### 🔹 PATCH - Partial Update User
- **Endpoint:** 'https://dummyjson.com/users/1'
- **Request Body:**
'''json
{
  "lastname": "QAEngineerPATCH"
}
- **Test:**
  - Status is 200
  - Validate only 'lastname' is changed
---

### 🔹 DELETE - Delete User
- **Endpoint:** 'https://dummyjson.com/users/1
- **Test:**
  - Status is 200
  - Response confirms deleted user data

---

## ▶️ How to Use This Collection

1. **Import Collection**
   Open Postman → Click 'Import' → Upload collection file.
   
3. **(Optional) Set Enviroment**
   Create enviroment with variables like 'base_url'.
   
4. **Run Individual Request**
   Select request → Click 'Send' → Observe the **Scripts** Tab.
   
5. **Export Collection**
   File → Export → Save collection for sharing or uploading to GitHub.

---

## 📝 Notes

- This project is focused on **manual API testing**, not automation frameworks.
- Two different public APIs are used to demonstrate different HTTP methods.
- Reqress supports only GET and POST; DummyJSON is used for more advanced testing like PUT, PATCH, and DELETE.

---

## 📌 Conclusion
This project demonstrates **manual QA testing with Postman** using two separate APIs dor different types of request methods.

---


