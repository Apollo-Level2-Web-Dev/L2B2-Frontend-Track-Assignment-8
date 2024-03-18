# Assignment-08 Frontend Path - 3

# **Cleaning Supplies Store Project Overview**

## **Disclaimer:**

> Welcome to the Cleaning Supplies Store platform. This project aims to develop the platform with enhanced features and UI/UX improvements tailored specifically for cleaning supplies enthusiasts. Leveraging technologies such as Next.js, and its features like Server-Side Rendering (SSR), Static Site Generation (SSG), Incremental Static Regeneration (ISR), the platform will serve as a dynamic marketplace for cleaning supplies. You have the flexibility to choose a niche within the cleaning supplies category such as Dishwashing Items, Laundry Products, Toilet Cleaners & Cleaning Accessories, Napkins & Paper Products, Pest Control Products, etc. However, ensure that the chosen niche is specific and aligned with the project's focus on cleaning supplies. This project emphasizes user engagement, seamless browsing, and an immersive shopping experience within the selected cleaning supplies niche.
> 

### **Project Overview:**

The Cleaning Supplies Store project aims to elevate user engagement and functionality within the cleaning supplies niche by incorporating key features and UI/UX enhancements. By leveraging cutting-edge technologies and design principles, the platform will deliver a seamless and immersive shopping experience, facilitating informed purchasing decisions and fostering long-term customer satisfaction among cleaning supplies enthusiasts.

### **Key Features Breakdown:**

In this project, you will be tasked with implementing the following key features and UI/UX enhancements tailored specifically for cleaning supplies enthusiasts:

1. **File-Based Routing:**
    - Implement file-based routing to ensure organized navigation and intuitive URL structures, enhancing overall user experience within the cleaning supplies niche.
2. **Static Site Generation (SSG):**
    - Utilize SSG to pre-render static pages, optimizing performance and enabling faster page loads for improved user engagement specifically for cleaning supplies listings.
3. **Incremental Static Regeneration (ISR):**
    - Employ ISR with a 30-second revalidation interval to update static pages incrementally, ensuring real-time data updates without compromising performance or scalability, thereby providing up-to-date information on cleaning supplies availability and specifications.
4. **Server-Side Rendering (SSR):**
    - Implement SSR to render dynamic content on the server, enhancing SEO capabilities and improving initial page load times for enhanced user experience, particularly for cleaning supplies details and comparisons.
5. **UI/UX Enhancements:**
    - Enhance the user interface with visually appealing components, intuitive navigation elements, and responsive design tailored to cleaning supplies enthusiasts' preferences, ensuring seamless browsing and exploration within the cleaning supplies niche.
6. **Server Components:**
    - Integrate server components to optimize rendering performance and facilitate efficient data fetching, ensuring a smooth user experience across different pages, especially for detailed cleaning supplies specifications and comparisons.
7. **Loading and Not Found Page:**
    - Design loading indicators to provide visual feedback during data fetching processes, enhancing user perception of responsiveness, and create a custom 404 (Not Found) page to gracefully handle invalid routes, guiding users back to relevant cleaning supplies listings.

# **Pages:**

## **Landing Page / Home Page: (”/”)**

*Showcase featured cleaning supplies items and promotions to capture user attention and encourage exploration within the cleaning supplies niche.*

1. **Navbar:**
    - Implement a navigation bar for easy access to different sections of the website, enhancing user navigation specifically for cleaning supplies categories and brands.
2. **Hero Section - Carousel with Product Image:**
    - Introduce a visually engaging hero section with a carousel showcasing key cleaning supplies items or promotions, enhancing aesthetic appeal and attracting cleaning supplies enthusiasts. (You can use either static images or dynamic images for carousel)
3. **Flash Sale:**
    - Implement **ISR** with a 30s revalidation.
    - Display top 4-6 flash sale cleaning supplies items, sorting based on product creation time, to highlight limited-time offers and encourage immediate purchase among cleaning supplies enthusiasts.
    - Each Product will have a flashSale property which will be a boolean value. On the basis of this value, flash sale products will be shown.
    - Provide a **"See All"** button to direct cleaning supplies enthusiasts to the **Flash Sale Products page (”/flash-sale”)** for comprehensive listings and details of discounted cleaning supplies items.
4. **Brands / Category:**
    - Show any random 6 Brands / Categories
    - Selecting brand / category depends on the niche of your project. For example, if your project is on Dishwashing Items, you can use categories like Dish Soap, Dishwasher Detergent, Dish Brush, etc.
    - You can use static data to create brand / categories
    - Make sure the static data of the brands / categories are available in your products data
    - Showcase top cleaning supplies brands or categories, allowing users to explore cleaning supplies items based on their preferences and interests within the cleaning supplies niche.
    - Enable cleaning supplies enthusiasts to access a dedicated page featuring all brands or categories for extensive browsing and selection within the cleaning supplies niche.
    - Clicking a Brand / Category will navigate to **All Products Page** with filtered data of that brand. **Example :** *(“/dishwashing-items?category=dish-soap”) or (“/laundry-products?category=detergent”)*
    - The route name for **All Products Page** will be dynamic depending on your niche. For example if your niche is Dishwashing Items, your route name for All Products page will be “/dishwashing-items”, “/dish-cleaning-supplies” or “/kitchen-cleaners”.
    - Use this query parameter to filter products on the basis of brand or category in the **All Products Page**
5. **Trending Products:**
    - Implement **ISR** with a 30s revalidation.
    - Show 6 Top Rated cleaning supplies items based on the ratings of your products
    - Display trending cleaning supplies items sorted by ratings to showcase popular items and facilitate user discovery within the cleaning supplies niche.
    - Highlight top-rated cleaning supplies items and provide a **"See All Products"** button for users to explore the complete product catalog, facilitating informed purchasing decisions.
6. **Footer:**
    - Include a clickable footer section with navigation links to essential pages such as
        - Trending Products
        - Categories/Brands
        - About Us
        - Contact Us
        - Customer Care

## **Flash Sale Products Page: (”/flash-sale”) [SSR]**

- Implement **Server-Side Rendering (SSR)**
- Present all flash sale cleaning supplies items with a countdown timer indicating the time remaining for each offer, fostering a sense of urgency and driving conversions among cleaning supplies enthusiasts.
- Implement a countdown timer on this page which will show the end time of the flash sale
- Countdown timer can be any time in minutes which will be dynamically / statically set.

## **All Products Page: (”/products”) [SSR]**

- The route name for All Products Page will be dynamic depending on your niche. For example if your niche is Dishwashing Items, your route name for All Products page will be **“/dishwashing-items”, “/dish-cleaning-supplies” or “/kitchen-cleaners”.**
- Implement filtering options based on rating, brand/category, and price range to streamline cleaning supplies items, enhancing user experience and satisfaction.

## **Single Product’s Detail Page: (”/products/:productId”) [SSR + SSG]**

- The route name for All Products Page will be dynamic depending on your niche. For example if your niche is Dishwashing Items, your route name for Products Details page will be **“/dishwashing-items/789”, “/dish-cleaning-supplies/123” or “/kitchen-cleaners/456”.**
- Implement both **Static Site Generation (SSG)** & **Server-Side Rendering (SSR)**
- Create **SSG for first 10 products** and do **SSR for rest of the products** available in your database.
- Create a detailed product page featuring
    - Images
    - Title
    - Price
    - Ratings
    - Brand / Category
    - Description

## **Dashboard : (”/dashboard”)**

- **Layout Design**
    - Use NextJS Layout feature to design the layout of the dashboard.
    - Implement a Sidebar for **All Products** navigation route.
- **All Products (”/dashboard/all-products”) [SSR]**
    - Implement **Server-Side Rendering (SSR)**
    - Provide a table view of all cleaning supplies items for easy management and navigation, tailored specifically for cleaning supplies listings.

# **Additional Information:**

1. **Code Implementation:**
    - Utilize Next.js with Typescript for efficient file-based routing and server-side rendering and optimizing performance specifically for cleaning supplies listings.
    - Implement NextJS Data Fetching technology ensuring a robust data flow tailored specifically for cleaning supplies browsing and comparison.
2. **Database Management:**
    - Choose MongoDB as the backend database, leveraging their capabilities for efficient data storage and retrieval.
    - Optionally, integrate Mongoose for defining database schemas and interacting with the database.
    - You can create a simple single page backend with Javascript.
3. **Improved UI/UX Design:**
    - Enhance the existing UI with responsive design, intuitive navigation, and visually appealing components tailored to cleaning supplies enthusiasts' preferences, ensuring seamless browsing and exploration within the cleaning supplies niche.
4. **Deployment:**
    - Deploy the application to a suitable hosting platform such as Vercel, [cyclic.sh](http://cyclic.sh/) or any ensuring accessibility and scalability specifically for cleaning supplies listings and comparisons.

### **Submission Guidelines:**

- Include a README file in both frontend and backend repositories explaining how to set up and use the application specifically for the Cleaning Supplies Store project.
- Provide the GitHub repository links for the frontend and backend, along with clear instructions for running the application locally, focusing specifically on cleaning supplies functionalities.
- Submit a live deployment link for the frontend application tailored specifically for cleaning supplies enthusiasts to facilitate evaluation.

### **Deadline:**

- 60 marks: February 24, 2024 11.59 PM
- 50 marks: March 25, 2024 11.59 PM
- No 30 Marks Deadline

### **Important Note:**

Plagiarism will not be tolerated. Ensure that the code you submit is your own work, tailored specifically for the Cleaning Supplies Store project. Any instances of plagiarism will result in 0 marks.

We wish you success with your assignment! Should you have any questions or require clarification, feel free to reach out for assistance.