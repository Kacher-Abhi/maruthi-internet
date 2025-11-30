# Maruthi Internet Website

A modern, mobile-responsive website for Maruthi Internet Service Provider serving Anekal, Chandapura, and Bommasandra areas in Bangalore.

## Features

- ✅ 6 Complete Pages (Home, Plans, Enterprise, Services, Pay, Help & Support)
- ✅ Fully Mobile Responsive Design
- ✅ Modern and Clean UI
- ✅ Easy Navigation
- ✅ Sticky Header
- ✅ Contact Form
- ✅ WhatsApp Support Link
- ✅ Google Maps Integration
- ✅ Payment Gateway Ready

## Pages Overview

1. **Home Page** (`index.html`)
   - Hero section with CTA
   - What we offer
   - Select your speed
   - Why choose us
   - Pricing packages
   - Customer reviews
   - Footer

2. **Plans Page** (`plans.html`)
   - Internet plans (50 Mbps to 500 Mbps)
   - Entertainment plans (Internet + TV bundles)

3. **Enterprise Plans** (`enterprise.html`)
   - Corporate plans
   - Internet leased line information

4. **Services Page** (`services.html`)
   - Fiber broadband
   - Satellite TV
   - Smart broadband
   - Ultra fast speed
   - 24/7 support
   - Affordable pricing

5. **Pay Page** (`pay.html`)
   - Payment gateway integration ready
   - Payment instructions
   - Multiple payment methods

6. **Help & Support** (`help-support.html`)
   - WhatsApp support link
   - About us section
   - Location map
   - Contact form

## Customization Guide

### 1. Update WhatsApp Link

In `help-support.html`, find the WhatsApp link and update it:

```html
<a href="https://wa.me/yournumber" class="btn btn-primary" target="_blank" id="whatsappLink">
```

Replace `yournumber` with your WhatsApp number in format: `91XXXXXXXXXX` (country code + number, no + or 0)
Example: `https://wa.me/919876543210`

### 2. Add Payment Gateway Link

In `pay.html`, find the pay button and update:

```html
<a href="#" class="btn btn-primary btn-large btn-pay" id="payButton">
```

Replace `#` with your payment gateway URL, or update the JavaScript in `script.js`:

```javascript
payButton.addEventListener('click', function(e) {
    e.preventDefault();
    window.location.href = 'YOUR_PAYMENT_GATEWAY_LINK_HERE';
});
```

### 3. Update Google Maps Location

In `help-support.html`, find the iframe and update the Google Maps embed URL:

```html
<iframe 
    src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3888.1234567890123!2d77.7000!3d12.8000!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x0!2zMTLCsDQ4JzAwLjAiTiA3N8KwNDInMDAuMCJF!5e0!3m2!1sen!2sin!4v1234567890123!5m2!1sen!2sin" 
    ...
</iframe>
```

To get your location's embed URL:
1. Go to Google Maps
2. Search for your location
3. Click "Share" → "Embed a map"
4. Copy the iframe code and replace the existing one

### 4. Update Contact Information

In `help-support.html`, update the office address:

```html
<div class="address-details">
    <p><strong>Maruthi Internet</strong></p>
    <p>Your Office Address Here</p>
    <p>Anekal, Bangalore</p>
    <p>Karnataka, India</p>
    <p><strong>Phone:</strong> +91 XXXXXXXXXX</p>
    <p><strong>Email:</strong> info@maruthiinternet.com</p>
</div>
```

### 5. Update Phone Number

In `help-support.html`, update the phone link:

```html
<a href="tel:+91XXXXXXXXXX" class="btn btn-outline">Call Now</a>
```

### 6. Update Email Address

In `help-support.html`, update the email link:

```html
<a href="mailto:support@maruthiinternet.com" class="btn btn-outline">Send Email</a>
```

### 7. Customize Colors (Optional)

In `styles.css`, you can customize the color scheme by updating the CSS variables:

```css
:root {
    --primary-color: #0066cc;
    --primary-dark: #0052a3;
    --secondary-color: #00a8e8;
    --accent-color: #ff6b35;
    /* ... other colors */
}
```

### 8. Update Pricing (if needed)

Update the pricing in:
- `index.html` (pricing section)
- `plans.html` (all plan cards)
- `enterprise.html` (enterprise plans)

## File Structure

```
Maruthi-website/
├── index.html          # Home page
├── plans.html          # Internet & Entertainment plans
├── enterprise.html     # Enterprise solutions
├── services.html       # Services page
├── pay.html            # Payment page
├── help-support.html   # Help & Support page
├── styles.css          # All styles
├── script.js           # JavaScript functionality
└── README.md           # This file
```

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Mobile Responsive

The website is fully responsive and works on:
- Desktop (1200px+)
- Tablet (768px - 1199px)
- Mobile (< 768px)

## Notes

- All images/icons are using emoji icons. You can replace them with actual images if needed.
- The contact form currently shows an alert. You'll need to integrate it with a backend service or email service (like Formspree, EmailJS, etc.) to actually send emails.
- The payment button needs to be connected to your payment gateway.
- Update the Google Maps embed with your actual location coordinates.

## Getting Started

1. Open `index.html` in a web browser to view the website
2. Customize the content as per your requirements
3. Update the links (WhatsApp, payment, map) as mentioned above
4. Deploy to your web hosting service

## Support

For any questions or customization help, please refer to the code comments or contact your developer.

---

**Built with ❤️ for Maruthi Internet**

