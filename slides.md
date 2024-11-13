---
theme: ./
highlighter: shiki
---

<div class="relative z-10">
    <h1>How to Build a <span class="gradient-text">$1 Million AI App</span> With <span class="orange-gradient-text"> <em>No Coding Background</em></span></h1>
</div>

<div class="qr-code"></div>
<div class="flex items-center justify-between relative z-10">
  <div class="flex-1">
    <p class="font-bold">Jason Chan</p>
    <p>Co-founder of memo.cards (Previously PDF2Anki)<br />Third Year Medical Student, LKS Faculty of Medicine, HKU<br />InnoTech HSBC Scholar<br />Cyberport Incubatee<br />Builder and AI Engineer</p>
  </div>
  <img src="/avatar.png" alt="Jason Chan" class="w-36 h-36 rounded-full ml-4">
</div>

<div class=" relative z-10">
  Press <KBD>space</KBD> to go to the next page ->
</div>

<div class="w-[800px] h-[800px] mx-auto absolute top-0 left-0 right-0 z-0">
  <Globe />
</div>

<Counter />

<div class="absolute bottom-0 right-0 ">
<FlappyBirdHome />
</div>

---

<div class="center-xy">
  <h1 class="text-8xl text-center ">hello everyone</h1>
</div>
<div class="qr-code"></div>
---

<div class="center-xy">
  <h1 class=" text-8xl text-center">and welcome to my workshop</h1>
</div>
<div class="qr-code"></div>
---

<div class="center-xy text-center">
   <h1>How to Build a <span class="gradient-text">$1 Million AI App</span> With <span class="orange-gradient-text"> <em>No Coding Background</em></span></h1>
</div>
<div class="qr-code"></div>
---

<div class="w-full h-full">
  <img src="/sus.webp"  alt="Suspicious" class="h-full w-full object-cover" />
</div>
<div class="qr-code"></div>

---

<div class="center-xy text-center">
   <h1>you are going to learn <span class="gradient-text">a lot of things</span> today</h1>
</div>
<div class="qr-code"></div>
---

<div class="w-full h-full flex items-center justify-center ">
  <img src="/bento.png" alt="Bento grid" class="w-full h-auto object-cover rounded-xl" />
</div>
<div class="qr-code"></div>

---

<div class="center-xy text-center">
   <h1>today it is going to be <span class="gradient-text">beginner</span> friendly</h1>
   <h2>yet we will be pushing the boundaries of what is possible with ai into some advanced concepts</h2>
</div>
<div class="qr-code"></div>
---

<div class="w-full h-full flex items-center justify-center">
  <img src="/cat.gif" alt="Cat having fun" class="w-full h-auto object-cover rounded-xl" />
</div>
<div class="qr-code"></div>

---

<div class="justify-center">
  <h1 class="text-8xl text-right text-red-500">Stop</h1>
  <h1 class="text-right">Join Menti ↓</h1>
</div>

<div class="absolute top-0 left-0 ">
<FlappyBird />
</div>
<Counter />
<div class="qr-code"></div>

---

<div class="center-xy">
  <h1 class="gradient-text text-10xl text-center ">Who Am I?</h1>
</div>
<div class="qr-code"></div>
---

<div class="center-xy">
  <h1 class="text-8xl text-center ">my name is <span class="gradient-text">jason chan</span></h1>
  <p class="text-center text-gray-500">@thetechjason</p>
</div>
<div class="qr-code"></div>
---

<div class="">
  <img src="/handstand.jpg"  alt="Full screen image" class="w-full h-full object-cover" />
  21 year old founder based in hk.
</div>
<div class="qr-code"></div>

---

# What We'll Be Doing Today

| Step | Description                                |
| ---- | ------------------------------------------ |
| 1    | Setting up our development environment     |
| 2    | Using AI to design our web app             |
| 3    | Implementing the design with AI assistance |
| 4    | Deploying our app to the internet          |

<h2 class="mt-3 font-bold">Let's get started!</h2>

<div class="qr-code"></div>

---

# Install a <span class="gradient-text">VPN</span>

| For Chrome **(Recommended)**                        | For macOS                                                 | For Windows                                                |
| --------------------------------------------------- | --------------------------------------------------------- | ---------------------------------------------------------- |
| 1. Open Chrome and go to Chrome Web Store           | 1. Go to https://protonvpn.com/download                   | 1. Go to https://protonvpn.com/download                    |
| 2. Search for "VPN Proxy VeePN"                     | 2. Click "Download ProtonVPN for macOS"                   | 2. Click "Download ProtonVPN for Windows"                  |
| 3. Click "Add to Chrome"                            | 3. Once downloaded, open the .dmg file                    | 3. Once downloaded, run the installer                      |
| 4. Click the VeePN icon in Chrome to set up and use | 4. Drag ProtonVPN into the Applications folder            | 4. Follow the installation wizard                          |
| 5. Click the VeePN icon in Chrome to set up and use | 5. Open ProtonVPN from Applications and set up an account | 5. Open ProtonVPN after installation and set up an account |

<Note>A VPN will help ensure the AI models we are using as well as Bolt works properly (from Hong Kong)</Note>

<div class="qr-code"></div>

---

# Go to <span class="gradient-text">www.bolt.new</span> and select <span class="orange-gradient-text">Next.js</span>

<div class="w-full h-full flex flex-col  items-center">
  <img src="/steps/step1.png"  alt="home screen of bolt.new with an arrow pointing to the next button" class="h-[500px]" />
</div>

<Note>A VPN will help ensure the AI models we are using as well as Bolt works properly</Note>

<div class="qr-code"></div>

---

<div class="w-full h-full flex flex-row justify-between items-start" >
  <div>
    <img src="/steps/step2.png"  alt="folder structure of a next.js app" class="w-[500px]" />
  </div>
<!-- table here -->
<div class="ml-4">
    <table class="border-collapse border border-gray-300">
      <thead>
        <tr>
          <th class="border border-gray-300 px-4 py-2">File/Folder</th>
          <th class="border border-gray-300 px-4 py-2">Purpose</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td class="border border-gray-300 px-4 py-2"><code>app</code></td>
          <td class="border border-gray-300 px-4 py-2">Main folder for your app's pages</td>
        </tr>
         <tr>
          <td class="border border-gray-300 px-4 py-2"><code>globals.css</code></td>
          <td class="border border-gray-300 px-4 py-2">Global CSS styles for the entire application</td>
        </tr>
        <tr>
          <td class="border border-gray-300 px-4 py-2"><code>layout.tsx</code></td>
          <td class="border border-gray-300 px-4 py-2">Root layout component for the app</td>
        </tr>
        <tr>
          <td class="border border-gray-300 px-4 py-2"><code>page.tsx</code></td>
          <td class="border border-gray-300 px-4 py-2">Main page component for the root route</td>
        </tr>
        <tr>
          <td class="border border-gray-300 px-4 py-2"><code>components</code></td>
          <td class="border border-gray-300 px-4 py-2">Folder for reusable React components</td>
        </tr>
        <tr>
          <td class="border border-gray-300 px-4 py-2"><code>hooks</code></td>
          <td class="border border-gray-300 px-4 py-2">Contains a custom toast hook</td>
        </tr>
        <tr>
          <td class="border border-gray-300 px-4 py-2"><code>package.json</code></td>
          <td class="border border-gray-300 px-4 py-2">Project dependencies and scripts</td>
        </tr>
      </tbody>
    </table>
  </div>
</div>
<div class="qr-code"></div>

---

<div class="center-xy">
  <h1 class=" text-center ">Hold up! I know this looks super overwhelming and scary</h1>
    <h3 v-click>... and it certainly was when I first got started</h3>
    <h3 v-click>... however, just like building muscle memory, the more you do it, the easier it gets</h3>
    <h3 v-click>so don't worry if you don't understand everything!</h3>
    <h3 v-click>just focus on having fun and getting hands on with ai-powered coding</h3>
</div>
<div class="qr-code"></div>

---

# Understanding <span class="orange-gradient-text">page.tsx</span> in Next.js

<div class="flex flex-col md:flex-row items-center justify-between space-y-8 md:space-y-0 md:space-x-8">
  <div class="text-lg space-y-2 md:w-1/2">
    <p>Think of <code>page.tsx</code> as the blueprint for your website's main page:</p>
    <ul class="list-disc list-inside space-y-2">
      <li>It's like the "welcome mat" of your website</li>
      <li>It decides what visitors see when they first arrive</li>
      <li>You can easily change what it shows, like updating a sign</li>
    </ul>
    <Note>Don't worry about the technical stuff yet - we'll use AI to help us work with it!</Note>
  </div>

  <div class="md:w-1/2">
    <img src="/welcomeSign.jpg" alt="Welcome sign" class="w-full h-auto rounded-lg shadow-lg" />
  </div>
</div>
<div class="qr-code"></div>

---

```typescript
export default function Home() {
    return (
        <div className="mt-5 ml-5 text-lg">Hello World! We are at HKU now!</div>
    );
}
```

| Code Element                      | Description                            |
| --------------------------------- | -------------------------------------- |
| `function Home()`                 | This is like a recipe for your page    |
| `return (...)`                    | This is what your page will show       |
| `<div>...</div>`                  | This is a container for your content   |
| `className="..."`                 | This adds styling to make it look nice |
| `Hello World! We are at HKU now!` | This is the actual text on your page   |

<div class="qr-code"></div>

---

# <span class="gradient-text">JavaScript</span> & <span class="orange-gradient-text">React</span> in a Nutshell

<div class=" space-y-6">
  <p><strong>JavaScript:</strong> The language that makes websites <strong>interactive</strong></p>
  <ul class="list-disc list-inside space-y-2">
    <li>Allows you to add <strong>behavior</strong> to your web pages</li>
    <li>Can <strong>respond</strong> to user actions (like clicks or typing)</li>
    <li>Can <strong>update</strong> the page without reloading</li>
  </ul>

  <p><strong>React:</strong> A popular JavaScript <strong>library</strong> for building user interfaces</p>
  <ul class="list-disc list-inside space-y-2">
    <li>Helps organize your code into <strong>reusable components</strong></li>
    <li>Makes it easier to build <strong>complex, interactive websites</strong></li>
    <li>Used by many <strong>big companies</strong> like Facebook and Instagram</li>
  </ul>
</div>
<div class="qr-code"></div>

---

# <span class="gradient-text">HTML</span> in a Nutshell

<div class="space-y-6 mb-4">
  <p><strong>HTML:</strong> The structure and content of web pages</p>
  <ul class="list-disc list-inside space-y-2">
    <li>Defines the <strong>basic building blocks</strong> of web pages</li>
    <li>Uses <strong>"tags"</strong> to <strong>mark up</strong> different types of content</li>
    <li>Examples: <strong>&lt;h1&gt;</strong> for headings, <strong>&lt;p&gt;</strong> for paragraphs, <strong>&lt;img&gt;</strong> for images</li>
  </ul>

</div>

```html
<h1>Welcome to My Website</h1>
<p>This is a paragraph of text.</p>
<img src="picture.jpg" alt="A beautiful landscape" />
```

<Note>HTML is like the skeleton of your website - it gives it structure!</Note>

<div class="qr-code"></div>

---

# <span class="gradient-text">Tailwind CSS</span> in a Nutshell

<div class="space-y-6 mb-6">
  <p><strong>Tailwind CSS:</strong> A tool for <strong>quickly styling</strong> your web pages</p>
  <ul class="list-disc list-inside space-y-2">
    <li>Provides <strong>pre-made classes</strong> for common styles</li>
    <li>Allows you to design <strong>without writing custom CSS</strong></li>
    <li>Makes it easy to create <strong>responsive</strong>, <strong>good-looking websites</strong></li>
  </ul>

</div>

```html
<div class="bg-gray-100 p-4 rounded-md">
    <p class="font-bold">Tailwind CSS Example:</p>
    <div class="bg-blue-500 text-white p-4 rounded-lg shadow-md">
        This is a styled box using Tailwind CSS classes
    </div>
</div>
```

<Note>Think of Tailwind as a big box of Lego pieces for styling your website!</Note>

<div class="qr-code"></div>

---

# A React Functional Component

<div class="space-y-2">
  <p>Let's create a simple component called <code>Greeting</code>:</p>
</div>

```jsx
function Greeting() {
  return (

  );
}

export default Greeting;
```

<div class="">
  <p>This is the basic structure of a React component:</p>
  <ul class="list-disc list-inside ">
    <li>It's a function</li>
    <li>It returns something (which will be our content)</li>
    <li>We export it so other parts of our app can use it</li>
  </ul>
</div>

<Note>Think of this as creating an empty box that we'll fill with content!</Note>

<div class="qr-code"></div>

---

```jsx
function Greeting() {
    return (
        <div>
            <h1>Welcome to My App!</h1>
            <p>This is a simple greeting component.</p>
            <button>Click me!</button>
        </div>
    );
}

export default Greeting;
```

<div class="">
  <p>We've added:</p>
  <ul class="list-disc list-inside">
    <li>A container <code>&lt;div&gt;</code></li>
    <li>A heading with <code>&lt;h1&gt;</code></li>
    <li>A paragraph with <code>&lt;p&gt;</code></li>
    <li>A button with <code>&lt;button&gt;</code></li>
  </ul>
</div>

<Note>This JSX looks like HTML, but it's actually JavaScript!</Note>

<div class="qr-code"></div>

---

```jsx
function Greeting() {
    return (
        <div className="p-6 max-w-sm mx-auto bg-white rounded-xl shadow-md">
            <h1 className="text-2xl font-bold text-blue-600 mb-2">
                Welcome to My App!
            </h1>
            <p className="text-gray-600 mb-4">
                This is a simple greeting component.
            </p>
            <button className="px-4 py-2 bg-blue-500 text-white rounded hover:bg-blue-600">
                Click me!
            </button>
        </div>
    );
}

export default Greeting;
```

 <div className="p-6 max-w-sm mx-auto bg-white rounded-xl shadow-md">
            <h1 className="text-2xl font-bold text-blue-600 mb-2">
                Welcome to My App!
            </h1>
            <p className="text-gray-600 mb-4">
                This is a simple greeting component.
            </p>
            <button className="px-4 py-2 bg-blue-500 text-white rounded hover:bg-blue-600">
                Click me!
            </button>
        </div>

<Note>Tailwind makes styling easy - just add classes to your elements!</Note>

<div class="qr-code"></div>

---

```typescript
export default function Home() {
    return (
        <div className="mt-5 ml-5 text-lg">Hello World! We are at HKU now!</div>
    );
}
```

<div class="qr-code"></div>

---

```typescript
export default function Home() {
    return (
        <div className="mt-5 ml-5 text-lg">Hello World! We are at HKU now!</div>
    );
}
```

<img src="/steps/padding.png" alt="image showing padding of 5 between the text and the edge of the screen" class="w-full h-auto rounded-xl" />

<div class="qr-code"></div>

---

# Install Dependencies

In the Bolt.new terminal, run:

```bash
npm install @blocknote/react @blocknote/mantine @blocknote/core
```

<img src="/steps/npmInstall.png" alt="Terminal output of npm install @blocknote/react @blocknote/mantine @blocknote/core" class="w-full h-auto rounded-lg shadow-md" />
<Note>This installs the necessary BlockNote packages</Note>

<div class="qr-code"></div>

---

# Create Editor Component

<p>Type in the following into the Bolt.new AI console: (make sure your VPN is on)</p>

<code>
Create an empty Editor component inside the components folder. DO not add any packages or modify package.json. Just add a placeholder text.
</code>

<img src="/steps/console.png" alt="Terminal output of creating Editor component" class="w-full h-auto rounded-lg shadow-md" />

<Note>React components can be reused across different pages</Note>

<div class="qr-code"></div>

---

Select all and replace `components/Editor.tsx`

<div style="height: 400px; overflow-y: auto;">

```typescript {all|9-11|12-19|20-70}
"use client"; // This registers <Editor> as a Client Component

import { Block, BlockNoteEditor, PartialBlock } from "@blocknote/core";
import "@blocknote/core/fonts/inter.css";
import { BlockNoteView } from "@blocknote/mantine";
import "@blocknote/mantine/style.css";
import { useEffect, useMemo, useState } from "react";

async function saveToStorage(jsonBlocks: Block[]) {
    localStorage.setItem("editorContent", JSON.stringify(jsonBlocks));
}

async function loadFromStorage() {
    // Gets the previously stored editor contents.
    const storageString = localStorage.getItem("editorContent");
    return storageString
        ? (JSON.parse(storageString) as PartialBlock[])
        : undefined;
}

export default function Editor() {
    const [initialContent, setInitialContent] = useState<
        PartialBlock[] | undefined | "loading"
    >("loading");

    // Loads the previously stored editor contents.
    useEffect(() => {
        loadFromStorage().then((content) => {
            setInitialContent(content);
        });
    }, []);

    // Creates a new editor instance.
    // We use useMemo + createBlockNoteEditor instead of useCreateBlockNote so we
    // can delay the creation of the editor until the initial content is loaded.
    const editor = useMemo(() => {
        if (initialContent === "loading") {
            return undefined;
        }
        return BlockNoteEditor.create({ initialContent });
    }, [initialContent]);

    if (editor === undefined) {
        return "Loading content...";
    }

    // Renders the editor instance.
    return (
        <BlockNoteView
            editor={editor}
            theme="light"
            onChange={() => {
                saveToStorage(editor.document);
            }}
        />
    );
}
```

</div>

<Note>This component will render our Notion-style editor</Note>

<div class="qr-code"></div>

---

# Update page.tsx

Now, let's update our `app/page.tsx` file:

```typescript {all|1|3|5-12}
import dynamic from "next/dynamic";

const Editor = dynamic(() => import("../components/Editor"), { ssr: false });

export default function Home() {
    return (
        <div className="p-5">
            <h1 className="text-2xl font-bold mb-4">Jason Notion App</h1>
            <Editor />
        </div>
    );
}
```

<Note>We use dynamic import to ensure BlockNote only loads on the client-side</Note>

<div class="qr-code"></div>

---

# Run Your App

If your app has not been running, in the Bolt.new terminal, run:

```bash
npm run dev
```

<Note>Congratulations! You've just integrated a complex library into your Next.js app!</Note>

<div class="qr-code"></div>

---

# Deploy Your App

Press the big <span class="gradient-text">Deploy</span> button in the top right corner of the screen.

<img src="/steps/deploy.png" alt="Terminal output of deploying app" class="w-full h-auto rounded-lg shadow-md" />

<div class="qr-code"></div>

---

<div class="center-xy">
  <h1 class=" text-center ">Congratulations!</h1>
    <h3 v-click>You've just built and deployed an AI-generated web app!</h3>
    <h3 v-click> Your app is now live at Netlify</h3>
    <h3 v-click>Register a Netlify account to ensure your website stays up after 2 weeks</h3>
</div>

<div class="qr-code"></div>

---

<div class="center-xy">
  <h1 class="text-center">Next steps</h1>
    <h3 v-click>Learn to use a dedicated IDE like Cursor for enhanced AI-powered coding</h3>
    <h3 v-click>Master Git and GitHub for version control and collaboration</h3>
    <h3 v-click>Explore hosting your projects with Vercel for seamless deployment</h3>
    <h3 v-click>Keep building, learning, and growing as a builder!</h3>
</div>

<div class="qr-code"></div>

---

# Thank You!

<div class="relative z-10 mt-32">
  <p class="font-bold">Jason Chan</p>
  <p>If you're interested in building for apps like this, we are currently hiring for full time, part time and internships at <a href="https://www.memo.cards">memo.cards</a>. More info at <a href="https://www.thelearningcompany.com/careers">thelearningcompany.com/careers</a></p>
  <p>I'm at most of the socials with: @thetechjason</p>
  <p><a href="https://techjason.com">techjason.com</a></p>
</div>

<div class="qr-code"></div>

<div class="w-[800px] h-[800px] mx-auto absolute top-0 left-0 right-0 z-0">
  <Globe />
</div>
