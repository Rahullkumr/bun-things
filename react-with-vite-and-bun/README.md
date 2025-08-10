# Bun + Vite + React

- This guide demonstrates how to use `Bun` as the package manager for a React project created with Vite.

- Official [Bun](https://bun.com/guides/ecosystem/vite) documentation 

- Official [Vite](j) documentation 
## Steps

1. Create a new Vite project with React template:
    
    ```sh
    bun create vite react-with-vite-and-bun
    ```
    - Then follow the prompts!
    
2. Change directory to your project:
    ```sh
    cd react-with-vite-and-bun
    ```
3. Install dependencies using Bun:
    ```sh
    bun install
    ```
4. Update the "dev" script in **package.json** to the following.

    ```diff
    - "dev": "vite",

    + "dev": "bunx --bun vite",
    ```
    - The `--bun` flag tells Bun to run Vite's CLI using `bun `instead of **node**
    - This starts the Vite dev server with HMR using Bun as runtime

4. Start the development server:
    ```sh
    bun run dev
    ```
5. Open your browser and go to `http://localhost:5173` to view your app.

## Why Bun + Vite + React Works So Well

- Bun accelerates dev workflows with its fast package management and bundling capabilities 

- Vite integrates seamlessly, serving React projects with modular hot reloading and optimized production builds 

- Together, they deliver a lightweight, high-performance experience for modern frontend development.