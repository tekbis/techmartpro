TechMartPro — store website (front-end)

HOW TO OPEN
Double-click index.html, or upload this whole folder to any static host
(Netlify, Vercel, GitHub Pages, cPanel). Keep the folder structure as is.

FILES
index.html      The whole site: styles, layout and code in one file
logo.png        Logo for light backgrounds
logo-white.png  Logo for the dark footer
img/            Product photos (800x800, white background) used on cards and product pages
cut/            Background-removed photos used in the hero slider

EDITING PRODUCTS
Open index.html and search for "CATALOG". Each product has:
  id, n (name), b (brand), cat (category), d (description),
  p (price), w (old price, or null), bd (badges: hot/sale/new),
  colors, st (storage/size options with extra price)
The product photo is img/<id>.jpg.

EDITING THE HERO
Search for "const HERO=[". Each slide has a product id (pid), big word (w),
background (c) and text (t). Hero photos are cut/<pid>.png (transparent PNG).

CHECKOUT
The checkout is a front-end design. It takes US addresses (state, ZIP, phone)
but does not charge cards. Connect a payment provider (e.g. Shopify, Stripe)
before going live, then remove the line "Online payments are not yet active".

Discount code for testing: WELCOME10

NEW FEATURES
- Sorting & filters on the shop (price, brand, on sale, price range)
- Wishlist (heart icon) — saved in the shopper's browser
- Compare up to 3 products side by side
- Recently viewed products
- Phone options: carrier, TechMartPro Care protection plans, add-on accessories
  (plan prices are placeholders — edit planFor() in index.html)
- Trade-in section with quote form (connect the form to your email/CRM to receive requests)
- Free-shipping suggestion in the cart
- 404 page, cookie notice, accessibility (keyboard focus, skip link, reduced motion)

BEFORE GOING LIVE
- og-image.jpg: social sites need a full URL. After you get a domain, change
  content="og-image.jpg" to e.g. content="https://yourdomain.com/og-image.jpg"
- Newsletter and trade-in forms need connecting to a service (e.g. Mailchimp, Formspree)
