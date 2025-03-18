<div>
<h1 style='text-align:center;'>Website Hosting</h1>
  
</div>



# Understanding Domains, DNS, and Protocols


## **1. What is a Domain?**

A **domain** is like the address of a website on the internet. Just like your home has a physical address, a website has a domain name to help people find it. For example:
- `google.com` is a domain name.
- `youtube.com` is another domain name.

Domains are easier to remember than the actual numerical addresses (called **IP addresses**) that computers use to locate websites. For example:
- Instead of typing `172.217.10.46` to access Google, you just type `google.com`.

Domains are organized into levels:
- **Top-Level Domain (TLD):** The last part of the domain, like `.com`, `.org`, `.net`.
- **Second-Level Domain (SLD):** The main part of the domain, like `google` in `google.com`.

---

## **2. What is DNS?**

**DNS (Domain Name System)** is like the phonebook of the internet. It translates human-friendly domain names (like `google.com`) into computer-friendly IP addresses (like `172.217.10.46`).

Here’s how it works:
1. You type a domain name (e.g., `google.com`) into your browser.
2. Your computer asks a DNS server, "What’s the IP address for `google.com`?"
3. The DNS server responds with the correct IP address.
4. Your browser connects to that IP address and loads the website.

Without DNS, you’d have to remember and type in long strings of numbers (IP addresses) to visit websites, which would be a hassle!

---

## **3. What are Protocols?**

**Protocols** are sets of rules that computers follow to communicate with each other over the internet. Think of them as the "languages" or "etiquette" that devices use to talk to each other.

Here are some common protocols:

### **a. HTTP (HyperText Transfer Protocol)**
- Used for loading websites in your browser.
- When you visit a website, your browser sends an HTTP request to the server, and the server sends back the website data.

### **b. HTTPS (HyperText Transfer Protocol Secure)**
- A secure version of HTTP.
- It encrypts the data sent between your browser and the server, so hackers can’t easily steal your information (like passwords or credit card details).

### **c. TCP/IP (Transmission Control Protocol / Internet Protocol)**
- The backbone of the internet.
- **TCP** ensures data is sent reliably and in the correct order.
- **IP** handles addressing and routing, so data gets to the right destination.

### **d. FTP (File Transfer Protocol)**
- Used for transferring files between computers over the internet.
- For example, uploading files to a website or downloading files from a server.

### **e. SMTP (Simple Mail Transfer Protocol)**
- Used for sending emails.
- When you send an email, your email client uses SMTP to deliver it to the recipient’s email server.

### **f. DNS (Domain Name System Protocol)**
- As mentioned earlier, DNS is also a protocol that helps translate domain names into IP addresses.

---

## **How It All Works Together**

1. You type a domain name (e.g., `google.com`) into your browser.
2. Your computer uses **DNS** to find the IP address of `google.com`.
3. Your browser uses **HTTP/HTTPS** to request the website data from the server at that IP address.
4. The server sends the website data back to your browser using **TCP/IP**.
5. Your browser displays the website for you to see.

---


# How to Host a Website Using GitHub Pages

Hosting a website using **GitHub Pages** is a simple and free way to publish your website online. GitHub Pages allows you to host static websites (HTML, CSS, JavaScript) directly from a GitHub repository. Here's a step-by-step guide:

---

## **Steps to Host a Website Using GitHub Pages**

### **1. Create a GitHub Account**
If you don’t already have a GitHub account, sign up at [github.com](https://github.com).

---

### **2. Create a New Repository**
1. Log in to your GitHub account.
2. Click the **+** icon in the top-right corner and select **New repository**.
3. Name your repository. For example: `my-website`.
   - If you want a personal website, name it `username.github.io` (replace `username` with your GitHub username).
   - For project websites, you can use any name.
4. Choose **Public** (GitHub Pages only works with public repositories for free).
5. Check the box **Add a README file** (optional but recommended).
6. Click **Create repository**.

---

### **3. Upload Your Website Files**
You need to upload your website files (HTML, CSS, JavaScript, etc.) to the repository.

#### **Option 1: Drag and Drop**
1. Open your repository on GitHub.
2. Drag and drop your website files into the repository.

#### **Option 2: Use Git Commands**
1. Install Git on your computer if you haven’t already: [git-scm.com](https://git-scm.com).
2. Open a terminal or command prompt.
3. Clone your repository to your computer:
   ```bash
   git clone https://github.com/username/repository-name.git

## Enter the following git Commands

```bash
  git add .
  git commit -m "Initial commit"
  git push origin main
```

### **4. Enable GitHub Pages**
1. Go to your repository on GitHub.
2. Click on the **Settings** tab.
3. Scroll down to the **Pages** section (on the left sidebar).
4. Under **Source**, select the branch where your website files are located (usually `main` or `master`).
5. Click **Save**.
6. Wait a few minutes, and GitHub will provide you with a URL for your website (e.g., `https://username.github.io/repository-name`).

---

### **5. Access Your Website**
- Once GitHub Pages is enabled, your website will be live at the provided URL.
- You can share this URL with others to access your website.

---

## **Tips for Using GitHub Pages**
- **Custom Domain:** You can use a custom domain (e.g., `www.yourdomain.com`) instead of the default GitHub Pages URL. Go to the **Pages** settings and add your custom domain.
- **Static Websites Only:** GitHub Pages only supports static websites (HTML, CSS, JavaScript). For dynamic websites (e.g., PHP, databases), you’ll need a different hosting service.
- **Jekyll Support:** GitHub Pages supports Jekyll, a static site generator. You can use Jekyll to create blogs or complex websites.
- **Automatic Updates:** Whenever you push changes to your repository, GitHub Pages will automatically update your website.


# How to Serve Websites Locally Using `http-server` and Python’s HTTP Server

Serving websites locally is a great way to test and develop your website before deploying it to a live server. Below, I’ll show you how to serve websites locally using two popular tools: **`http-server` (Node.js)** and **Python’s built-in HTTP server**.

---

## **1. Using `http-server` (Node.js)**

`http-server` is a simple, zero-configuration command-line HTTP server. It’s great for serving static files (HTML, CSS, JavaScript).

### **Steps to Use `http-server`**

#### **1. Install Node.js and npm**
1. Download and install Node.js from [nodejs.org](https://nodejs.org).
2. Verify the installation by running these commands in your terminal:
   ```bash
   node -v
   npm -v

3. Install http-server using nodejs
```bash
npm install -g http-server
```
4.Navigate to the directory containing the folder files and enter the following command

```bash
http-server

```
