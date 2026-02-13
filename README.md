# **OpenRouter API Tester ⚡️**

A lightweight, clean, and secure web interface to quickly test AI models via the [OpenRouter](https://openrouter.ai) API.

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

## **🧩 How it Works (Under the Hood)**

The entire application lives in a single index.html file. Here is a breakdown for developers:

1. **Styles**: We use **Tailwind CSS** via CDN. This allows us to style the page using utility classes directly in the HTML without a separate CSS file or build process.  
2. **Icons**: **Font Awesome** (via CDN) provides the UI icons (robot, user, shields).  
3. **JavaScript Logic**:  
   * **No Frameworks**: Pure Vanilla JS handles DOM manipulation and event listeners.  
   * **API Interaction**: The fetch() API sends POST requests to https://openrouter.ai/api/v1/chat/completions.  
   * **State Management**: A simple messageHistory array tracks the conversation context in memory.  
   * **Error Handling**: Custom logic catches specific OpenRouter errors (like 429 Rate Limits or Data Policy requirements) to show helpful toasts instead of generic console errors.

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
