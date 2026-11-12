# Mission 5 - Phase 1 - Individual Assignment

## Trade Me Auction CLI

This project is a command-line auction application built using **Node.js** and **MongoDB**.

The purpose of this project is to demonstrate how a NoSQL database can be used to store and manage auction item data. The application uses a CLI (Command Line Interface) to interact with the auction data.

---

## Technologies Used

- Node.js
- MongoDB
- MongoDB Compass
- MongoDB Node.js Driver
- JavaScript
- Command Line Interface (CLI)

---

## Project Setup

### 1. Install Node.js

Download and install Node.js from:

https://nodejs.org/

Check that Node.js is installed:

```bash
node --version
```

Check npm:

```bash
npm --version
```

---

### 2. Install MongoDB

MongoDB Community Server is required to run the database locally.

The MongoDB server runs on the default local port:

```text
27017
```

The MongoDB server is configured to run locally on:

```text
mongodb://127.0.0.1:27017
```

---

### 3. Install MongoDB Compass

MongoDB Compass can be used to view and manage the database using a graphical interface.

Connect to:

```text
mongodb://127.0.0.1:27017
```

After connecting, the auction database and its collection can be viewed in Compass.

---

## Installing the Project

Open PowerShell or a terminal in the project folder.

Install the project dependencies:

```bash
npm install
```

The MongoDB Node.js driver is included as a project dependency.

If required, it can be installed with:

```bash
npm install mongodb
```

---

## Running the Auction CLI

The application is controlled through the command line.

### Seed Auction Data

To add the sample auction data to MongoDB:

```bash
node scripts/auction-cli.js seed
```

Expected result:

```text
Auction data seeded successfully.
```

This command creates the auction items in the MongoDB database.

---

### Delete Auction Data

To delete the auction items from MongoDB:

```bash
node scripts/auction-cli.js delete
```

Expected result:

```text
3 auction items deleted.
```

This removes the auction items from the database.

---

## MongoDB Database

The application uses MongoDB as a NoSQL database.

The database stores auction item information in a collection.

Example auction information can include:

- Item name
- Description
- Starting price
- Current bid
- Seller
- Auction information

MongoDB stores the data as documents rather than rows and columns like a traditional relational database.

MongoDB Compass can be used to check that the data has been successfully added or deleted.

---

## CLI

CLI stands for **Command Line Interface**.

Instead of using a graphical interface, commands are entered into the terminal to interact with the application.

For example:

```bash
node scripts/auction-cli.js seed
```

The CLI sends the required operation to the application, which then interacts with MongoDB.

---

## Testing the Application

The application can be tested by running the CLI commands and checking the MongoDB database using MongoDB Compass.

### Seed Test

Run:

```bash
node scripts/auction-cli.js seed
```

Then open MongoDB Compass and check that the auction documents have been added.

### Delete Test

Run:

```bash
node scripts/auction-cli.js delete
```

Then check MongoDB Compass again to confirm that the auction documents have been removed.

---

## Project Structure

```text
mission-5-phase-1/
│
├── scripts/
│   └── auction-cli.js
│
├── package.json
├── package-lock.json
└── README.md
```

The main CLI file is:

```text
scripts/auction-cli.js
```

This file contains the commands used to interact with the auction data.

---

## How to Run the Project

1. Make sure MongoDB is running.
2. Open the project folder in PowerShell or a terminal.
3. Install the dependencies:

```bash
npm install
```

4. Seed the auction data:

```bash
node scripts/auction-cli.js seed
```

5. Open MongoDB Compass and check the database.

6. When finished, delete the test auction data:

```bash
node scripts/auction-cli.js delete
```

---

## Learning Outcomes

Through this project I learned how to:

- Set up and use MongoDB locally.
- Connect a Node.js application to MongoDB.
- Use the MongoDB Node.js driver.
- Store data in a NoSQL database.
- Retrieve and manage database information through a CLI.
- Use MongoDB Compass to view database data.
- Test database operations using command-line commands.
- Document a project using a README file.

---

## Conclusion

Mission 5 Phase 1 demonstrates a basic Trade Me-style auction system using Node.js, a command-line interface, and MongoDB.

The project shows how auction data can be stored and managed using a NoSQL database and how a CLI can be used to perform database operations.
