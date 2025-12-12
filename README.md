
# Capital City Quiz

A simple and fun quiz web app where users guess the capital city of a randomly shown country. The score updates based on correct answers, and a new country appears after each attempt.

---

## One-line Description

A fast, interactive game that tests how well you know world capitals.

---

## Demo

Example:

<img width="1920" height="968" alt="Screenshot (324)" src="https://github.com/user-attachments/assets/d6ac3533-3138-4d7f-9f14-43ca2f9d5a4c" />


---

## Features

* Displays a random country each round
* User inputs the capital and submits their guess
* Score increases for each correct answer
* Clean UI with playful background
* Real-time feedback
* Responsive design

---

## Tech Stack

* **Frontend:** HTML, CSS, JavaScript
* **Backend:** Node.js, Express
* **Database:** PostgreSQL
* **HTTP Client:** Axios

---

## How It Works

1. App loads a random country from your database.
2. User enters what they believe is the capital.
3. Backend verifies the answer.
4. Score updates instantly.
5. New country appears automatically.

---

## Installation

Clone the repo:

```bash
git clone https://github.com/<your-username>/Flag_Quiz.git
cd Flag_Quiz
```

Install dependencies:

```bash
npm install
```

Set up environment variables in `.env`:

```
DB_HOST=localhost
DB_USER=postgres
DB_PASSWORD=yourpassword
DB_NAME=capitals
DB_PORT=5432
```

Start the server:

```bash
node index.js
```

Visit the app at:

```
http://localhost:3000
```

---

## Project Structure (example)

```
project/
├── public/
│   ├── styles.css
│   └── script.js
├── views/
│   └── index.ejs
├── database/
│   └── capitals.sql
├── index.js
├── package.json
└── README.md
```

---

## API Endpoints

### `GET /`

Renders the quiz page with a random country.

### `POST /submit`

Checks whether the answer is correct and returns:

```json
{
  "correct": true,
  "score": 5,
  "nextCountry": "Spain"
}
```

---

## Future Improvements

* Add timer mode
* Add leaderboard
* Add difficulty levels
* Add country flag display

---
