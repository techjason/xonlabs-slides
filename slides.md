---
theme: ./
highlighter: shiki
---

# How to Build a <span class="gradient-text">$1 Million AI App</span> in <span class="orange-gradient-text">1 Hour</span> With _No Coding Background_

<div class="qr-code"></div>

<div class="">
  <p class="font-bold">Jason Chan</p>
  <p>Co-founder of memo.cards (Previously PDF2Anki)<br />Third Year Medical Student, LKS Faculty of Medicine, HKU<br />InnoTech HSBC Scholar<br />Cyberport Incubatee<br />Builder and AI Engineer</p>
</div>

<div class="pt-6">
  Press <KBD>space</KBD> to go to the next page ->
</div>

---

# What We'll Be Doing Today

| Step | Description                                |
| ---- | ------------------------------------------ |
| 1    | Setting up our development environment     |
| 2    | Using AI to design our web app             |
| 3    | Implementing the design with AI assistance |
| 4    | Deploying our app to the internet          |

<h2 class="mt-3font-bold">Let's get started!</h2>

---

# Step 1: Install Google Chrome

| Step | Action                                                         |
| ---- | -------------------------------------------------------------- |
| 1    | Open your current web browser                                  |
| 2    | Go to https://www.google.com/chrome/                           |
| 3    | Click the "Download Chrome" button                             |
| 4    | Once downloaded, run the installer                             |
| 5    | Follow the on-screen instructions to complete the installation |

<Note>Chrome will be our primary browser for this project</Note>

---

# Step 2: Create a GitHub Account

| Step | Action                                                       |
| ---- | ------------------------------------------------------------ |
| 1    | Open Google Chrome                                           |
| 2    | Go to https://github.com/                                    |
| 3    | Click "Sign up" in the top-right corner                      |
| 4    | Enter your email address then create a password and username |
| 5    | Click "Create account"                                       |

<Note>GitHub will be used to store and manage our code</Note>

---

# Step 3: Install Git

| For macOS                                                          | For Windows                                       |
| ------------------------------------------------------------------ | ------------------------------------------------- |
| 1. Open Terminal (press Cmd + Space, type "Terminal", press Enter) | 1. Go to https://git-scm.com/download/win         |
| 2. Type `git --version` and press Enter                            | 2. The download should start automatically        |
| 3. If Git is not installed, you'll be prompted to install it       | 3. Once downloaded, run the installer             |
|                                                                    | 4. Accept the default options during installation |

<Note>Git is a tool that helps manage code changes</Note>

---

# Step 4: Install Node.js and npm

| Step | Action                                                        |
| ---- | ------------------------------------------------------------- |
| 1    | Go to https://nodejs.org/                                     |
| 2    | Download the "LTS" (Long Term Support) version                |
| 3    | Run the installer once downloaded                             |
| 4    | Follow the installation wizard, accepting the default options |
| 5    | Restart your computer after installation                      |

<Note>Node.js and npm are required to run and manage JavaScript projects</Note>

---

# Step 5: Install Cursor IDE

| Step | Action                                                         |
| ---- | -------------------------------------------------------------- |
| 1    | Go to https://cursor.sh/                                       |
| 2    | Click the "Download" button                                    |
| 3    | Once downloaded, run the installer                             |
| 4    | Follow the on-screen instructions to complete the installation |

<Note>Cursor IDE is an AI-powered code editor that will help us write code</Note>

---

# Step 6: Sign Up for Vercel

| Step | Action                                         |
| ---- | ---------------------------------------------- |
| 1    | Go to https://vercel.com/                      |
| 2    | Click "Sign Up" in the top-right corner        |
| 3    | Choose "Continue with GitHub"                  |
| 4    | Authorize Vercel to access your GitHub account |
| 5    | Complete the sign-up process                   |

<Note>Vercel will be used to deploy our web app for free</Note>

---

# Step 7: Sign Up for v0.dev

| Step | Action                                                              |
| ---- | ------------------------------------------------------------------- |
| 1    | Go to https://v0.dev/                                               |
| 2    | Click "Sign Up" or "Get Started"                                    |
| 3    | Follow the sign-up process                                          |
| 4    | You may need to join a waitlist (approval usually takes a few days) |

<Note>v0.dev is an AI tool that will help us design our web app</Note>

---

# Step 8: Create a New Project Folder

| Step | Action                                                       |
| ---- | ------------------------------------------------------------ |
| 1    | Open File Explorer (Windows) or Finder (macOS)               |
| 2    | Navigate to a location where you want to create your project |
| 3    | Create a new folder called "my-ai-app"                       |

<Note>This folder will contain all the files for our web app</Note>

---

# Step 9: Open the Project in Cursor IDE

| Step | Action                                                         |
| ---- | -------------------------------------------------------------- |
| 1    | Open Cursor IDE                                                |
| 2    | Click "File" > "Open Folder"                                   |
| 3    | Navigate to and select the "my-ai-app" folder you just created |
| 4    | Click "Select Folder"                                          |

<Note>Cursor IDE is now set up with our project folder</Note>

---

# Step 10: Initialize a New Next.js Project (Part 1)

| Step | Action                                                |
| ---- | ----------------------------------------------------- |
| 1    | In Cursor IDE, open the terminal (View > Terminal)    |
| 2    | In the terminal, type: `npx create-next-app@latest .` |
| 3    | Press Enter and wait for the command to finish        |

<Note>This starts the process of setting up a new Next.js project in our folder</Note>

---

# Step 10: Initialize a New Next.js Project (Part 2)

| Step | Action                                                       |
| ---- | ------------------------------------------------------------ |
| 4    | Answer the prompts as follows:                               |
|      | - Would you like to use TypeScript? → Yes                    |
|      | - Would you like to use ESLint? → Yes                        |
|      | - Would you like to use Tailwind CSS? → Yes                  |
|      | - Would you like to use `src/` directory? → No               |
|      | - Would you like to use App Router? → Yes                    |
|      | - Would you like to customize the default import alias? → No |

<Note>This completes the setup of our new Next.js project</Note>

---

# Step 11: Run the Development Server

| Step | Action                                             |
| ---- | -------------------------------------------------- |
| 1    | In the Cursor IDE terminal, type: `npm run dev`    |
| 2    | Press Enter                                        |
| 3    | Wait for the message "Ready in X.Xs"               |
| 4    | Open Google Chrome and go to http://localhost:3000 |
| 5    | You should see the default Next.js page            |

<Note>Your local development server is now running!</Note>

---

# Step 12: Design Your App with v0.dev

| Step | Action                                                     |
| ---- | ---------------------------------------------------------- |
| 1    | Open a new tab in Chrome and go to https://v0.dev/         |
| 2    | Log in if necessary                                        |
| 3    | In the prompt box, describe the web app you want to create |
| 4    | Wait for v0.dev to generate the design                     |
| 5    | Explore the design and make any desired changes            |

<Note>v0.dev will create a visual design based on your description</Note>

---

# Step 13: Implement the Design

| Step | Action                                                                    |
| ---- | ------------------------------------------------------------------------- |
| 1    | In v0.dev, click "Copy Code" to get the React component code              |
| 2    | Go back to Cursor IDE                                                     |
| 3    | Open the file `app/page.tsx`                                              |
| 4    | Delete the existing content                                               |
| 5    | Paste the copied code from v0.dev                                         |
| 6    | Use Cursor's AI features to help understand and modify the code if needed |

<Note>We're now implementing the AI-generated design in our app</Note>

---

# Step 14: Customize Your App

| Step | Action                                               |
| ---- | ---------------------------------------------------- |
| 1    | In Cursor IDE, explore the pasted code               |
| 2    | Use Cursor's AI to ask questions about the code      |
| 3    | Make any desired changes to customize your app       |
| 4    | Save the file (Ctrl+S or Cmd+S)                      |
| 5    | Check http://localhost:3000 to see your changes live |

<Note>Cursor's AI can help explain and modify the code</Note>

---

# Step 15: Commit Your Changes

| Step | Action                                               |
| ---- | ---------------------------------------------------- |
| 1    | In Cursor IDE, open the terminal                     |
| 2    | Type the following commands:                         |
|      | ```                                                  |
|      | git add .                                            |
|      | git commit -m "Initial commit with AI-generated app" |
|      | ```                                                  |
| 3    | Press Enter after each command                       |

<Note>This saves your changes to Git</Note>

---

# Step 16: Create a GitHub Repository

| Step | Action                                                                          |
| ---- | ------------------------------------------------------------------------------- |
| 1    | Go to https://github.com/                                                       |
| 2    | Click the "+" icon in the top-right, then "New repository"                      |
| 3    | Name your repository "my-ai-app"                                                |
| 4    | Leave it public and don't initialize with any files                             |
| 5    | Click "Create repository"                                                       |
| 6    | Copy the commands under "…or push an existing repository from the command line" |

<Note>This creates a place to store your code online</Note>

---

# Step 17: Push Your Code to GitHub

| Step | Action                                                      |
| ---- | ----------------------------------------------------------- |
| 1    | Go back to Cursor IDE                                       |
| 2    | In the terminal, paste the commands you copied from GitHub  |
| 3    | Press Enter to run the commands                             |
| 4    | Refresh your GitHub repository page to see your code online |

<Note>Your code is now stored on GitHub</Note>

---

# Step 18: Deploy Your App with Vercel

| Step | Action                                      |
| ---- | ------------------------------------------- |
| 1    | Go to https://vercel.com/                   |
| 2    | Click "Add New..." > "Project"              |
| 3    | Find and select your "my-ai-app" repository |
| 4    | Click "Deploy"                              |
| 5    | Wait for the deployment to complete         |

<Note>Vercel is now hosting your web app online</Note>

---

# Congratulations!

You've just built and deployed an AI-generated web app!

-   Your app is now live at the URL provided by Vercel
-   You can continue to make changes and push to GitHub
-   Vercel will automatically update your live site

<div class="pt-6">
  <p class="font-bold">Next Steps:</p>
  <p>1. Customize your app further</p>
  <p>2. Learn more about React and Next.js</p>
  <p>3. Explore more AI tools for development</p>
</div>

---

# Thank You!

<div class="">
  <p class="font-bold">Jason Chan</p>
  <p>Co-founder of memo.cards (Previously PDF2Anki)<br />Third Year Medical Student, LKS Faculty of Medicine, HKU<br />InnoTech HSBC Scholar<br />Cyberport Incubatee<br />Builder and AI Engineer</p>
</div>

<div class="pt-6">
  <p>Follow me for more tutorials:</p>
  <p>@thetechjason</p>
</div>

<div class="qr-code"></div>
