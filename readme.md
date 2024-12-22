# Landing Page Prototype

## Public IP Address/URL
- [Landing Page](http://your-public-ip)  
  *(Replace `http://your-public-ip` with the actual IP address or domain.)*

## Overview
This project demonstrates setting up a simple web server and deploying a landing page. It showcases my ability to provision a server, configure networking, and deploy web content.

## Steps to Recreate
### 1. Provision the Server
- Used AWS EC2 to create a virtual machine with Ubuntu.
- Configured a security group to allow ports:
  - **22**: SSH access.
  - **80**: HTTP traffic.
  - **443**: HTTPS traffic (optional for SSL).

### 2. Install the Web Server
- Installed **Nginx** using the following commands:
  ```bash
  sudo apt update && sudo apt install nginx -y
  ```

### 3. Deploy HTML Page
- Created an `index.html` file with the project details:
  ```html
  <!DOCTYPE html>
  <html lang="en">
  <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <title>Welcome to Ahmad Zayyanu Landing Page</title>
  </head>
  <body>
      <h1>Welcome to Ahmad Zayyanu's Landing Page</h1>
      <p>Project Title: Landing Page Prototype</p>
      <p>Description: A prototype demonstrating server provisioning and web application deployment.</p>
      <h2>About Me</h2>
      <p>Ahmad Zayyanu is a software engineering student...</p>
  </body>
  </html>
  ```

### 4. Networking Configuration
- Configured the security group on AWS to allow HTTP (port 80).
- Verified accessibility via browser using the public IP address.

### 5. Bonus: HTTPS Setup (Optional)
- Installed **Certbot**:
  ```bash
  sudo apt install certbot python3-certbot-nginx -y
  ```
- Secured the website with an SSL certificate.

## Deliverables
- **Public IP Address/URL:** `http://your-public-ip`
- **Screenshot:** 
  ![Landing Page Screenshot](screenshot.png)

## Notes
- Replace the `index.html` content to personalize your page.
- Ensure the server firewall rules are updated for accessibility.
