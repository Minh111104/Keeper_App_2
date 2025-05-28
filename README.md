# dKeeper

**dKeeper** is a decentralized note-taking web application (upgraded from Keeper App 1). Built with **React** and **Material UI** for the frontend and powered by the **Internet Computer Protocol (ICP)** through DFINITY's SDK and `dfx`, this app allows users to add and delete notes in a decentralized environment.

## ✨ Features

- Add new notes with a title and content
- Delete notes
- Fully responsive, clean Material UI design
- Backend deployed on the Internet Computer via DFX

## 🧰 Technologies Used

- React
- Material UI (`@mui/material`, `@mui/icons-material`)
- Vite
- DFINITY SDK (`dfx`)
- Internet Computer (ICP)
- Canister backend written in Motoko (or Rust if applicable)

## 🚀 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v14 or higher recommended)
- [DFX SDK](https://smartcontracts.org/docs/quickstart/quickstart-intro.html)
- [npm](https://www.npmjs.com/)

### Installation

1. **Clone the repository:**

   ```sh
   git clone <your-repo-url>
   cd dkeeper
   ```

2. **Install dependencies:**

   ```sh
   npm install
   ```

3. **Start the local Internet Computer replica:**

   ```sh
   dfx start --background
   ```

4. **Deploy the canisters:**

   ```sh
   dfx deploy
   ```

5. **Start the React development server:**

   ```sh
   npm run dev
   ```

6. **Open your browser:**

   ```sh
   http://localhost:5173
   ```

## 🌐 Local Canister Access

After deploying with `dfx deploy`, you can also access the app from:

```sh
http://localhost:8000?canisterId=<canister_id>
```

## 📌 Notes on Frontend Environment

If you're hosting frontend code outside of the DFX ecosystem, ensure:

- `NODE_ENV` is set to `"production"`
- Your build process handles `process.env.NODE_ENV` replacements
- You write a custom `createActor()` if needed for accessing canisters

## 📚 Documentation & Resources

- [DFINITY SDK Quick Start](https://smartcontracts.org/docs/quickstart/quickstart-intro.html)
- [Motoko Language Guide](https://smartcontracts.org/docs/language-guide/motoko.html)
- [JavaScript Agent API Reference](https://smartcontracts.org/docs/javascript-reference/index.html)

## 📄 License

This project is developed for educational purposes and learning decentralized app development on the Internet Computer.
