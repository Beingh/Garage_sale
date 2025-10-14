BACKYARD SALE WEBSITE - USER GUIDE
====================================

SETUP INSTRUCTIONS:
-------------------
1. Place all your product images in the "images" folder
2. Open index.html in any web browser to view the website
3. The website works on Windows, Android, iOS, and all devices with a web browser


HOW TO ADD A NEW PRODUCT:
-------------------------
1. Open index.html
2. Find the section marked "<!-- PRODUCT 1 - COPY FROM HERE -->"
3. Copy everything from that comment to "<!-- TO HERE FOR ADDING NEW PRODUCTS -->"
4. Paste it at the bottom before the closing </main> tag
5. Update:
   - Change onclick="navigateToProduct('product1.html')" to your new product page (e.g., 'product4.html')
   - Change the image src to your new product image
   - Change the product name
   - Change the original price and sale price
6. Create a new product page by copying any existing product page (e.g., product1.html)
7. Rename it to match your new product (e.g., product4.html)
8. Update the content in your new product page


HOW TO ADD MORE IMAGES TO A PRODUCT:
-------------------------------------
1. Open the product page (e.g., product1.html)
2. Find the images array in the <script> section at the bottom
3. Add new image paths like this:
   const images = [
       'images/product1.jpg',
       'images/product1-2.jpg',
       'images/product1-3.jpg',
       'images/product1-4.jpg'  // <-- Just add your new image here
   ];


HOW TO ADD MORE DESCRIPTION BULLET POINTS:
-------------------------------------------
1. Open the product page (e.g., product1.html)
2. Find the description section with <ul> tags
3. Copy this section:
   <!-- COPY FROM HERE TO ADD MORE BULLET POINTS -->
   <li>Feature or description point 1</li>
   <!-- TO HERE -->
4. Paste it where you want the new bullet point
5. Change the text to your new description point


HOW TO UPDATE CONTACT INFORMATION:
-----------------------------------
1. In all HTML files (index.html and all product pages), find the footer section
2. Update:
   - Phone number: Change "8237256620" in the phone link
   - Google Maps: Replace "YOUR_GOOGLE_MAPS_LINK_HERE" with your actual Google Maps link
     (To get this: Open Google Maps, find your location, click "Share", copy the link)
   - WhatsApp: Change "918237256620" to your WhatsApp number (include country code 91)


HOW TO UPDATE PRODUCT ID:
--------------------------
1. Open the product page
2. Find this section:
   <div class="product-id">
       <strong>Product ID:</strong> <span class="id-value">ENTER_PRODUCT_ID_HERE</span>
   </div>
3. Replace "ENTER_PRODUCT_ID_HERE" with your actual product ID


COLOR THEME:
------------
The website uses a green and white color theme as requested.
- Primary green: #2d7a3e
- Background: white (#ffffff)


HOSTING THE WEBSITE:
--------------------
You can host this website for free on:
1. GitHub Pages (https://pages.github.com/)
2. Netlify (https://www.netlify.com/)
3. Vercel (https://vercel.com/)

Simply upload all the files to any of these platforms.


FOLDER STRUCTURE:
-----------------
public/
  ├── index.html (Home page with product grid)
  ├── product1.html (Product 1 details)
  ├── product2.html (Product 2 details)
  ├── product3.html (Product 3 details)
  ├── styles.css (All styling)
  ├── script.js (JavaScript functions)
  └── images/ (Put all product images here)

IMPORTANT NOTES:
----------------
- All prices display in Indian Rupees (₹)
- The website is fully responsive and works on all devices
- No database required - everything is in simple HTML files
- To add products, just copy and paste the marked sections
- Keep your image files small (under 1MB each) for faster loading
