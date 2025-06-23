# 🚀 Jest Express API Testing Example

This repository provides a complete example of how to **test a Node.js Express API using Jest**. It demonstrates **unit testing**, **integration testing**, and **API testing** with high code coverage.

[![Tests](https://img.shields.io/badge/tests-passing-brightgreen)](https://github.com/thamerh/jest-express-api-testing-example)
[![Coverage](https://img.shields.io/badge/coverage-95.83%25-blue)](#coverage)
[![Jest](https://img.shields.io/badge/tested%20with-jest-99424f.svg)](https://jestjs.io)

---

## 🧩 Table of Contents

- [📁 Project Structure](#-project-structure)
- [⚙️ Prerequisites](#️-prerequisites)
- [📦 Installation](#-installation)
- [🚀 Running the API](#-running-the-api)
- [🧪 Testing the Code](#-testing-the-code)
- [📊 Generating Coverage Reports](#-generating-coverage-reports)
- [✅ Git Hook Scripts](#-git-hook-scripts)
- [📸 Coverage Screenshot](#-coverage-screenshot)
- [🙌 Credits](#-credits)

---

## 📁 Project Structure

.
├── README.md
├── package.json
├── package-lock.json
├── src
│ ├── controller.js
│ ├── index.js
│ ├── router.js
│ └── service.js
└── test
├── controller.test.js
├── index.test.js
├── router.test.js
└── service.test.js

yaml
Copy
Edit

---

## ⚙️ Prerequisites

- Node.js (v18.17.1 or higher)
- npm (comes with Node.js)

> Recommended: Use [nvm](https://github.com/nvm-sh/nvm) to manage Node.js versions.

---

## 📦 Installation

```bash
git clone https://github.com/thamerh/jest-express-api-testing-example.git
cd jest-express-api-testing-example
npm install
🚀 Running the API
Start the Express server:

bash
Copy
Edit
npm start
Test the API endpoint using curl or any HTTP client:

bash
Copy
Edit
curl http://localhost:3000/posts
🧪 Testing the Code
This project uses Jest for testing. To run all tests:

bash
Copy
Edit
npm test
Example output:

bash
Copy
Edit
PASS  test/router.test.js
PASS  test/controller.test.js
PASS  test/service.test.js
PASS  test/index.test.js
📊 Generating Coverage Reports
To generate a full test coverage report:

bash
Copy
Edit
npm run coverage
It will generate output in the terminal and a detailed report in:

bash
Copy
Edit
coverage/lcov-report/index.html
Example output:

pgsql
Copy
Edit
---------------|---------|----------|---------|---------|-------------------
File           | % Stmts | % Branch | % Funcs | % Lines | Uncovered Line #s 
---------------|---------|----------|---------|---------|-------------------
All files      |   95.83 |      100 |   85.71 |   95.83 |                   
 controller.js |     100 |      100 |     100 |     100 |                   
 index.js      |   83.33 |      100 |       0 |   83.33 | 9                 
 router.js     |     100 |      100 |     100 |     100 |                   
 service.js    |     100 |      100 |     100 |     100 |                   
✅ Git Hook Scripts
This project uses Husky for Git hooks. A pre-commit hook ensures tests run before every commit.

Example:

bash
Copy
Edit
$ git commit -am 'feat: add basic husky support'

> jest test/**.test.js

PASS  test/index.test.js
PASS  test/service.test.js
PASS  test/router.test.js
PASS  test/controller.test.js

Made with ❤️ by Shikhar.
