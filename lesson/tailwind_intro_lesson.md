# 🧱 Tailwind CSS

## 🔹 What is Tailwind CSS?
- **Tailwind CSS** is a utility-first CSS framework that simplifies web development by providing a set of pre-designed utility casses.
- It allows you to build custom designs without writing custom CSS
- It promotes consistency, scalability, and efficiency.

---

## 🔹 What are the key advantages to using Tailwind CSS?
- **Tailwind CSS** removes the need for complex class names
- It minimizes your CSS code
- Allows for easy customization without adding additional CSS
- **Tailwind CSS** was created with built-in responsiveness. The utility classes of **Tailwind CSS** are optimized for responsiveness, which allows for easy mobile-friendly layouts

---

## 🔹 How do you use Taiwind CSS in your project?
- **Taiwind CSS** allows for easy styling by combining many single purpose presentational classes called utility classes.
- These utility classes are added directly to the elements markup
- an example of setting up an h1 heading would be: `<h1 class='text-3xl text-red-500 underline'>`
- We will go over some of the common utility classes in the lab.

---

## 🔹 HELPFUL VSCODE PLUGIN
- A helpful plugin for using **Tailwind CSS** in VSCode is called [Tailwind CSS IntelliSense](https://marketplace.visualstudio.com/items?itemName=bradlc.vscode-tailwindcss)
- This plugin will show suggested utility classes for your HTML elements.

---

## 🔹 How to setup Tailwind CSS in my project? 
- There are a few different ways to get Tailwind set up in your project. The easiest and most direct way to do it is to use a Tailwind CDN in a `<link>` element within the `<head>` of your HTML page. 

`<link rel="stylesheet" href="https://unpkg.com/tailwindcss@^2/dist/tailwind.min.css">`
- This will tell your HTML to ignore normal element styling and to use the utility classes withn each element.
