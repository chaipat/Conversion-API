# Conversion-API
Conversion-API

To install the Facebook Conversion API, you need to follow a series of steps to set up the necessary components and configure your website or server to send events directly to Facebook's servers. Here's a detailed guide to help you through the process:


## Step 1: Create a Facebook Business Manager Account

If you don't already have a Facebook Business Manager account, you need to create one:

- Go to [business.facebook.com.](https://business.facebook.com/)
- Click "Create Account."
- Follow the prompts to set up your account.



##   Step 2: Create a Facebook Pixel

- In your Facebook Business Manager, go to "Business Settings."
- Under "Data Sources," select "Pixels."
- Click "Add" and follow the instructions to create a new pixel.
- Note down the Pixel ID, as you will need it later.

##   Step 3: Generate Access Token

- Go to the [Events Manager.](https://www.facebook.com/events_manager2/list/pixel/)
- Select your Pixel and click "Settings."
- Scroll down to the "Conversions API" section.
- Click "Generate Access Token" and note down the token.

##  Step 4: Set Up Server-Side Code

Depending on your server environment (Node.js, PHP, Python, etc.), you'll need to write code to send events to Facebook. Below are examples for Node.js and PHP.

## Step 5: Verify Events in Events Manager

- Go to [Events Manager.](https://www.facebook.com/events_manager2/list/pixel/)
- Select your Pixel.
- Under "Test Events," enter your website URL and start testing to see if events are being received correctly.

##  Step 6: Monitor and Optimize

- Monitor the received events in the Events Manager.
- Adjust the data being sent as needed to ensure accurate and comprehensive tracking.

By following these steps, you will have set up the Facebook Conversion API to send 
server-side events directly to Facebook. This method helps you ensure that event tracking is accurate and resilient against browser-based limitations like ad blockers.

## User Data Parameters

| Parameters | Description |
| ----------------- | ------------------------------------------------------------------ |
| Email (em) | The user's email address, hashed using SHA-256. |
| Phone (ph) | The user's phone number, hashed using SHA-256. |
| Gender (ge) | The user's gender, "f" for female and "m" for male, hashed using SHA-256. |
| Date of Birth (db) | The user's date of birth in YYYYMMDD format, hashed using SHA-256. |
| Last Name (ln) | The user's last name, hashed using SHA-256. |
| First Name (fn) | The user's first name, hashed using SHA-256. |
| City (ct) | The user's city, hashed using SHA-256. |
| State (st) | The user's state, hashed using SHA-256. |
| ZIP Code (zp) | The user's ZIP code, hashed using SHA-256. |
| Country (country) | The user's country, hashed using SHA-256. |
| External ID (external_id) | Any unique ID from the advertiser, such as a loyalty membership ID, user ID, or cart ID. |
| Client IP Address (client_ip_address) | The IP address of the user, not hashed. |
| Client User Agent (client_user_agent) | The user agent string of the user's browser, not hashed. |
| FBC (fbc) | The Facebook click ID, which comes from fbclid URL parameter. |
| FBP (fbp) | The Facebook browser ID value, which comes from the _fbp cookie. |
| Subscription ID (subscription_id) | The subscription ID for the user in your system.|
| FB Login ID (fb_login_id) | The Facebook ID of the user if they logged in via Facebook Login. |


## Standard Event Names

| Event Names | Description |
| ----------------- | ------------------------------------------------------------------ |
| AddPaymentInfo | When a user adds payment information during a checkout process. |
| AddToCart | When a user adds an item to their shopping cart. |
| AddToWishlist | When a user adds an item to their wishlist. |
| CompleteRegistration |  When a user completes a registration form on your website. |
| Contact | When a user contacts your business. |
| CustomizeProduct | When a user customizes a product. |
| Donate | When a user makes a donation to your organization. |
| FindLocation | When a user searches for your business's location. |
| InitiateCheckout | When a user initiates the checkout process. |
| Lead | When a user submits information to indicate interest in your product or service (e.g., form submission). |
| Purchase | When a user completes a purchase on your website. |
| Schedule | When a user books an appointment with your business. |
| Search | When a user performs a search on your website. |
| StartTrial | When a user starts a free trial of your product or service. |
| SubmitApplication | When a user submits an application for a product, service, or program. |
| Subscribe | When a user subscribes to your service. |
| ViewContent | When a user views a piece of content on your website, such as a product page. |
