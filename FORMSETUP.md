# Contact Form Setup Instructions

## How to Receive Messages via Formspree

Your contact form is now set up to use Formspree, a free service that forwards form submissions to your email.

### Step 1: Create a Formspree Account

1. Go to [https://formspree.io](https://formspree.io)
2. Sign up for a free account (you can use your email: patrickzlw@outlook.com)
3. Verify your email address

### Step 2: Create a New Form

1. After logging in, click "New Form"
2. Formspree will generate a unique form ID (looks like: `xrgjnbqk` or `ynoqwkpd`)
3. Copy this form ID

### Step 3: Update Your HTML File

1. Open `index.html`
2. Find this line (around line 318):
   ```html
   <form class="contact-form" id="contactForm" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```
3. Replace `YOUR_FORM_ID` with your actual Formspree form ID
4. Example: If your form ID is `xrgjnbqk`, it should look like:
   ```html
   <form class="contact-form" id="contactForm" action="https://formspree.io/f/xrgjnbqk" method="POST">
   ```

### Step 4: Test the Form

1. Save the file
2. Open `index.html` in your browser
3. Fill out and submit the contact form
4. Check your email (the one you used to sign up for Formspree)
5. You should receive the message!

### Step 5: Customize Email Settings (Optional)

In your Formspree dashboard, you can:
- Customize the email subject line
- Add email forwarding
- Set up auto-replies
- View submission history
- Export submissions

### Free Plan Limits

- Free plan: Up to 50 submissions per month
- Paid plans: Available if you need more submissions

### Alternative: EmailJS (Frontend-only)

If you prefer not to use Formspree, you can use EmailJS instead. It's also free and works entirely from the frontend without a backend.

### Alternative: Netlify Forms

If you deploy your site to Netlify, you can use Netlify Forms (also free and easy to set up).

---

**Note:** After you update the form action URL with your Formspree form ID, the contact form will start sending messages to your email automatically!
