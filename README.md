# Contact Me Form

This project implements a "Contact Me" form that allows users to send messages directly to your email using the [EmailJS](https://www.emailjs.com/) API. It includes a styled form for user input and a custom JavaScript function that handles email sending with feedback for successful or failed submissions.

## Features

- **Form Validation**: Required fields include `first name`, `last name`, `email`, and `message`.
- **Email Sending with EmailJS**: The form uses EmailJS for sending emails directly from the browser.
- **Success and Error Feedback**: Users receive a success message upon successful submission or an error message if sending fails.
- **Custom Button with SVG Animation**: The "Send" button includes an SVG icon and custom animation.

## Setup and Usage

### Prerequisites

1. [EmailJS account](https://www.emailjs.com/) - Register and create a public key, service ID, and template ID for this project.
2. [SweetAlert](https://sweetalert.js.org/) - For user-friendly success/error alerts.

### Installation

1. Clone the repository or download the project files.
2. Open the project folder and insert your EmailJS credentials:
    - Replace `"PUBLIC KEY"` in `script.js` with your actual EmailJS public key.
    - Replace `"SERVICE ID"` and `"TEMPLATE ID"` with your service and template IDs.

### Configuration

Edit the JavaScript in `script.js` to include your EmailJS credentials:

```javascript
emailjs.init("YOUR_PUBLIC_KEY"); // Replace with your EmailJS public key
emailjs.send("YOUR_SERVICE_ID", "YOUR_TEMPLATE_ID", {
    first_name: firstName,
    last_name: lastName,
    email: emailAddress,
    message: message,
});
```

### How to Use

1. Fill out the form fields (First Name, Last Name, Email Address, and Message).
2. Click the "Send" button to submit.
3. Upon submission, you will receive a success message if the email is sent successfully, or an error message if it fails.

### Dependencies

- **EmailJS**: To send the email.
- **SweetAlert**: For success/error alert pop-ups.
- **Font Awesome** and **Boxicons**: For SVG icons and styling.


## This project is open source. Feel free to modify and distribute.

---

Let me know if you'd like any changes!