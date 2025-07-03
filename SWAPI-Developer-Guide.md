# SWAPI Developer Guide

*Sample API documentation created for freelance technical writing portfolio.*

---

## 📌 What is SWAPI?

The **Star Wars API (SWAPI)** is a free, open REST API providing data about the Star Wars universe:
- Characters
- Films
- Planets
- Species
- Starships
- Vehicles  

🌐 [https://swapi.dev](https://swapi.dev)

---

## 🌐 Base URL
```
https://swapi.dev/api/
```

---

## 🔐 Authentication

No authentication or API key is required.

---

## 📖 Endpoints Overview

| Resource   | Endpoint Example |
|------------|-----------------|
| People     | `/people/` |
| Films      | `/films/` |
| Planets    | `/planets/` |
| Species    | `/species/` |
| Starships  | `/starships/` |
| Vehicles   | `/vehicles/` |

---

## 🚀 Example Requests

### List people (characters)

```http
GET https://swapi.dev/api/people/
```

Sample response:
```json
{
  "count": 82,
  "next": "https://swapi.dev/api/people/?page=2",
  "previous": null,
  "results": [
    {
      "name": "Luke Skywalker",
      "height": "172",
      "mass": "77"
      // ...
    }
  ]
}
```

---

### Get details of a specific character

```http
GET https://swapi.dev/api/people/1/
```

---

### Pagination

Responses contain `next` and `previous` links to navigate pages.

---

## ⚠️ Error Handling

- `200 OK` — Success
- `404 Not Found` — The resource does not exist
- `500 Internal Server Error` — Server error

---

## 🧑‍💻 Example in Python

```python
imp
