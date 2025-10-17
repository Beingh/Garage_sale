MOBILE ACCESSORIES WEBSITE - USER GUIDE
==========================================

SETUP INSTRUCTIONS:
-------------------
1. Place all your product images in the "images" folder
2. Open index.html in any web browser to view the website
3. The website works on Windows, Android, iOS, and all devices


WEBSITE STRUCTURE (3 PAGES):
-----------------------------
PAGE 1: Categories (index.html)
- Shows all product categories in a grid
- Click any category to view products in that category

PAGE 2: Products List (e.g., chargers.html, cables.html)
- Shows all products in the selected category
- Displays product image, name, crossed original price, and sale price
- Click any product to view detailed information
- Back button returns to categories

PAGE 3: Product Details (e.g., product-charger-1.html)
- Shows product images with forward/backward navigation
- Displays product ID, prices, and detailed description
- Back button returns to products list


HOW TO ADD A NEW CATEGORY:
---------------------------
1. Open index.html
2. Find the section marked "<!-- CATEGORY 1 - COPY FROM HERE -->"
3. Copy everything from that comment to "<!-- TO HERE FOR ADDING NEW CATEGORIES -->"
4. Paste it at the bottom before the closing </main> tag
5. Update:
   - Change onclick="navigateToCategory('chargers.html')" to your new category page
   - Change the category icon (use emoji or icon)
   - Change the category name and description
6. Create a new category page by copying any existing category page (e.g., chargers.html)
7. Rename it to match your new category


HOW TO ADD A NEW PRODUCT TO A CATEGORY:
----------------------------------------
1. Open the category page (e.g., chargers.html)
2. Find the section marked "<!-- PRODUCT 1 - COPY FROM HERE -->"
3. Copy everything from that comment to "<!-- TO HERE FOR ADDING NEW PRODUCTS -->"
4. Paste it at the bottom before the closing </main> tag
5. Update:
   - Change onclick="navigateToProduct('product-charger-1.html')" to your new product page
   - Change the image src to your new product image
   - Change the product name
   - Change the original price and sale price
6. Create a new product detail page by copying any existing product page
7. Rename it to match your new product
8. Update the back button link to point to the correct category page


HOW TO ADD MORE IMAGES TO A PRODUCT:
-------------------------------------
1. Open the product detail page (e.g., product-charger-1.html)
2. Find the images array in the <script> section at the bottom
3. Add new image paths like this:
   const images = [
       'images/charger1.jpg',
       'images/charger1-2.jpg',
       'images/charger1-3.jpg',
       'images/charger1-4.jpg'  // <-- Just add your new image here
   ];


HOW TO ADD MORE DESCRIPTION BULLET POINTS:
-------------------------------------------
1. Open the product detail page
2. Find the description section with <ul> tags
3. Copy this section:
   <!-- COPY FROM HERE TO ADD MORE BULLET POINTS -->
   <li>Your description text here</li>
   <!-- TO HERE -->
4. Paste it where you want the new bullet point
5. Change the text to your new description


HOW TO UPDATE PRODUCT ID:
--------------------------
1. Open the product detail page
2. Find this section:
   <div class="product-id">
       <strong>Product ID:</strong> <span class="id-value">ENTER_PRODUCT_ID_HERE</span>
   </div>
3. Replace "ENTER_PRODUCT_ID_HERE" with your actual product ID


HOW TO UPDATE CONTACT INFORMATION:
-----------------------------------
1. In all HTML files, find the footer section
2. Update:
   - Phone number: Change "8237256620" in the phone link
   - Google Maps: Replace "YOUR_GOOGLE_MAPS_LINK_HERE" with your actual Google Maps link
     (To get this: Open Google Maps, find your location, click "Share", copy the link)
   - WhatsApp: Change "918237256620" to your WhatsApp number (include country code 91)


IMAGE NAMING CONVENTION:
-------------------------
- Category images: Use descriptive names (e.g., charger1.jpg, cable1.jpg)
- Product images:
  - Main image: productname.jpg (e.g., charger1.jpg)
  - Additional images: productname-2.jpg, productname-3.jpg (e.g., charger1-2.jpg)


COLOR THEME:
------------
The website uses a green and white color theme:
- Primary green: #2d7a3e
- Background: white (#ffffff)
- Accent: light green (#f0f9f2)


FOLDER STRUCTURE:
-----------------
mobile-accessories/
  ├── index.html (Categories page)
  ├── chargers.html (Chargers category products)
  ├── cables.html (Cables category products)
  ├── earphones.html (Earphones category products)
  ├── product-charger-1.html (Product detail page)
  ├── product-cable-1.html (Product detail page)
  ├── styles.css (All styling)
  ├── script.js (JavaScript functions)
  └── images/ (All product images)


NAVIGATION FLOW:
----------------
Categories Page → Products Page → Product Detail Page
     ↑               ↑                    ↑
     └───────────────┴────────────────────┘
         (Back buttons allow easy navigation)


HOSTING THE WEBSITE:
--------------------
You can host this website for free on:
1. GitHub Pages (https://pages.github.com/)
2. Netlify (https://www.netlify.com/)
3. Vercel (https://vercel.com/)

Simply upload all the files to any of these platforms.


IMPORTANT NOTES:
----------------
- All prices display in Indian Rupees (₹)
- The website is fully responsive and works on all devices
- No database required - everything is in simple HTML files
- To add products/categories, just copy and paste the marked sections
- Keep your image files small (under 1MB each) for faster loading
- Test on mobile devices to ensure proper display
