# **OpenRouter API Tester ⚡️**

A lightweight, clean, serverless, and secure web interface to quickly test AI models via the [OpenRouter](https://openrouter.ai) API.

Built as a **single HTML file**, it requires no installation, build steps, or backend server.

## **✨ Features**

* **Zero Setup**: Just open the file in your browser.  
* **Privacy First**: Your API Key and chats are **never saved** (neither on a server nor in the browser). Everything happens in the current session's volatile memory.  
* **Free Model Support**: Correctly handles specific errors for free models (e.g., Data Policy, Rate Limits).  
* **Modern Design**: Clean Light Mode theme built with Tailwind CSS.  
* **Direct Connection**: API calls go directly from your browser to OpenRouter.

## **🚀 How to Use**

### **Method 1: Online (GitHub Pages)**

If you have enabled GitHub Pages for this repository, simply visit your site's link.

### **Method 2: Local**

1. Download the index.html file (or clone this repository).  
2. Open index.html with any modern browser (Chrome, Firefox, Edge, Safari).  
3. Enter your OpenRouter **API Key**.  
4. Enter the **Model ID** (e.g., google/gemini-2.0-flash-exp:free).  
5. Start chatting\!

## **🛠 Technologies**

* HTML5  
* JavaScript (Vanilla, ES6+)  
* Tailwind CSS (via CDN)  
* Font Awesome (Icons)

## **⚠️ Security Note**

This application is designed for **client-side** use.

* Ensure you use the app over a secure connection (HTTPS) or locally.  
* Never enter personal or sensitive data in chats with LLM models.

*Open Source Educational Project for testing OpenRouter APIs.*
