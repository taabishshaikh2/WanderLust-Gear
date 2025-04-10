# WanderLust-Gear

README: Recommended Products Section - Wanderlust Gear
Overview
This project implements a Recommended Products section within the Wanderlust Gear Shopify theme. The section dynamically fetches and displays products based on metafields, enhancing user experience and product discoverability.
Features
•	Dynamic Product Recommendations: Fetch and display up to 10 recommended products based on metafield values.
•	Flickity Slider Integration: Displays four products at a time with smooth navigation.
•	Randomized Selection: Products are randomly selected from metafield-based recommendations on each page load.
•	Responsive Design: Ensures seamless experience across mobile and desktop.
•	Performance Optimized: Implements lazy loading for images and optimized queries for faster page load.
•	Error Handling & Loading Indicators: Displays appropriate messages for missing data or errors.
•	GitHub Integration: The project is version-controlled and hosted on a GitHub repository.
Coding Approach
1. Section Creation
•	Created a new Liquid section: recommended-products.liquid.
•	Added schema settings to allow merchants to configure the section in the Shopify theme editor.
2. Fetching Recommended Products
•	Used Shopify's product.metafields.custom.recommended_products to retrieve product IDs.
•	Utilized Shopify's all_products global object to fetch product details dynamically.
•	Implemented logic to shuffle products randomly on each page load.
3. Display Logic
•	Used a Flickity carousel for smooth scrolling.
•	Rendered product cards dynamically with key details (image, title, price, add-to-cart button).
4. Error Handling & Loading Optimization
•	Implemented loading indicators to enhance UX.
•	Used Liquid's conditional checks to handle missing metafield data gracefully.
•	Optimized queries to ensure efficient fetching of data.
5. Delivery Estimates (Pincode Mapping)
Added an estimated delivery feature for product pages using predefined pincode-based estimates:
const deliveryEstimates = {
    "400001": "3-5 days", "400059": "3-5 days", "400080": "3-5 days", // Mumbai
    "110001": "5-7 days", "110085": "5-7 days", "110092": "5-7 days", // Delhi
    "560001": "7-10 days", "560034": "7-10 days", "560100": "7-10 days", // Bangalore
    "411001": "4-6 days", "411038": "4-6 days", "411057": "4-6 days"  // Pune
};
6. GitHub Repository
•	The entire theme modifications, including the Recommended Products section and other enhancements, are version-controlled and pushed to GitHub.
•	A structured commit history ensures easy tracking of changes and improvements.
Future Enhancements
•	Use AI-based recommendations instead of metafields for better personalization.
•	Optimize queries further using Shopify's Storefront API for faster load times.
•	Improve accessibility with better keyboard navigation support in the slider.
Installation & Usage
1.	Clone the GitHub repository:
2.	git clone https://github.com/your-repo-name.git
3.	Upload the theme to Shopify.
4.	Enable the "Recommended Products" section in the theme customizer.
5.	Add product metafields for recommendations.
Contribution
Feel free to fork the repository and contribute by submitting pull requests!
________________________________________
This README provides a structured explanation of the approach, making it easier for developers to understand and contribute.

