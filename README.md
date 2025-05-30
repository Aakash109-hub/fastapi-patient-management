# 🏥 FastAPI Patient Management System

A beginner-friendly **Patient Management System API** built using **FastAPI**. This project demonstrates how to perform full **CRUD operations** using RESTful endpoints and **Pydantic** for data validation.

It also includes computed fields like **BMI** and **health verdict** based on patient data.

---

## 📌 Features

- ✅ Create, Read, Update, Delete (CRUD) patient records
- 📊 Computed fields for BMI and health verdict using Pydantic's `@computed_field`
- 🔍 Sort patients by height, weight, or BMI (ascending or descending)
- 💡 JSON-based data storage (simple and file-driven)
- ⚡ Built with FastAPI for high performance and simplicity

---

## 🚀 Technologies Used

- [FastAPI](https://fastapi.tiangolo.com/) — Web framework
- [Pydantic](https://docs.pydantic.dev/) — Data validation and parsing
- Python 3.10+

---

## 🧠 Endpoints Overview

| Method | Endpoint             | Description                          |
|--------|----------------------|--------------------------------------|
| GET    | `/`                  | Welcome message                      |
| GET    | `/about`             | API description                      |
| GET    | `/view`              | View all patient records             |
| GET    | `/patient/{id}`      | View a single patient by ID          |
| GET    | `/sort`              | Sort patients by `height`, `weight`, or `bmi` |
| POST   | `/create`            | Create a new patient record          |
| PUT    | `/edit/{id}`         | Update patient info                  |
| DELETE | `/delete/{id}`       | Delete a patient record              |

---

## 🛠️ How to Run Locally

1. **Clone the repo**
```bash
git clone https://github.com/Aakash109-hub/fastapi-patient-management.git
cd fastapi-patient-management
````

2. **Install dependencies**

```bash
pip install fastapi uvicorn
```

3. **Create a `patients.json` file**

```json
{}
```

4. **Run the app**

```bash
uvicorn main:app --reload
```

5. **Test it in your browser**
   Visit [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs) for the Swagger UI.

---

## 🗃️ Sample Patient Object (POST Body)

```json
{
  "id": "P001",
  "name": "Aakash",
  "city": "Pune",
  "age": 28,
  "gender": "male",
  "height": 1.75,
  "weight": 70
}
```

---

## 📚 Learning Highlights

* Used FastAPI's path, query, and body parameters
* Applied Pydantic's `@computed_field` for dynamic field calculation (BMI, verdict)
* Performed data validation using constraints (e.g., `gt`, `lt`, `Literal`)
* Implemented sorting logic via query parameters
* Practiced exception handling and API response formatting

---

## 🙌 Acknowledgment

This project is part of my journey to learn FastAPI and build real-world backend systems. Feedback and suggestions are welcome!
