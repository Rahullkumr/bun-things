# React + Vite + Bun

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
    - This allows you to take advantage of Bun's performance benefits
    
4. Start the development server:
    ```sh
    bun run dev
    ```
5. Open your browser and go to `http://localhost:5173` to view your app.