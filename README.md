# 🎶 Musician Hire Platform  

**Musician Hire Platform** is a responsive and user-friendly website designed to help users connect with talented musicians for events, gatherings, or personal projects. Developed as part of an internship assignment, the platform features **pricing cards**, **embedded audio tracks**, and an easy-to-use **contact form** integrated with **EmailJS** for seamless communication.  

---

## 🚀 Features  

- **Pricing Cards**: Clear and attractive pricing plans for hiring musicians.  
- **Audio Tracks**: Preview sample music directly on the platform.  
- **Responsive Design**: Optimized for desktop and mobile devices.  
- **Contact Form Integration**: Use **EmailJS** to send inquiries directly from the website.  
- **Interactive UI**: Built with HTML, CSS, and jQuery for smooth user interactions.  

---

## 🌟 Tech Stack  

- **Frontend**: HTML, CSS, jQuery  
- **Form Handling**: EmailJS integration  
- **Styling**: Custom CSS and CDN-based libraries for additional UI components  
- **Hosting**: Vercel  

---

## 📧 Contact Form Setup  

1. Sign up at [EmailJS](https://emailjs.com).  
2. Create a service and template in the EmailJS dashboard.  
3. Copy the service ID, template ID, and public key to integrate with the contact form.  
4. Use the following code snippet in your `script.js`:  

```javascript  
emailjs.init('YOUR_PUBLIC_KEY');  

$('#contact-form').on('submit', function (e) {  
    e.preventDefault();  
    emailjs.sendForm('YOUR_SERVICE_ID', 'YOUR_TEMPLATE_ID', this)  
        .then(() => alert('Message sent successfully!'))  
        .catch((error) => alert('Failed to send message:', error));  
});  
```  

