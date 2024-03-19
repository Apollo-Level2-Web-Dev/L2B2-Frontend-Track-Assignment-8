# Assignment-08 Frontend Path - 1

# **Electronic Gadgets Shop Project Overview**

## **Disclaimer:**

> Welcome to  the Electronic Gadgets Shop platform. This project aims to develop the platform with enhanced features and UI/UX improvements tailored specifically for electronic gadgets enthusiasts. Leveraging technologies such as **Next.js**, and its features like **Server-Side Rendering (SSR)**, **Static Site Generation(SSG), Incremental Static Regeneration (ISR),** the platform will serve as a **dynamic marketplace for electronic devices** (for example you can choose any from these categories Mobiles/Laptops/TV/Refrigerators etc.). You can also choose any niche related to electronic gadgets on your own. But keep the niche very much specific like we have mentioned earlier. This project emphasizes user engagement, seamless browsing, and an immersive shopping experience within the electronic gadgets niche.
> 

### **Project Overview:**

The Electronic Gadgets Shop project aims to elevate user engagement and functionality within the electronic gadgets niche by incorporating key features and UI/UX enhancements. By leveraging cutting-edge technologies and design principles, the platform will deliver a seamless and immersive shopping experience, facilitating informed purchasing decisions and fostering long-term customer satisfaction among electronic gadgets enthusiasts.

### **Key Features Breakdown:**

In this project, you will be tasked with implementing the following key features and UI/UX enhancements tailored specifically for electronic gadgets enthusiasts:

1. **File-Based Routing:**
    - Implement file-based routing to ensure organized navigation and intuitive URL structures, enhancing overall user experience within the electronic gadgets niche.
2. **Static Site Generation (SSG):**
    - Utilize SSG to pre-render static pages, optimizing performance and enabling faster page loads for improved user engagement specifically for electronic gadgets listings.
3. **Incremental Static Regeneration (ISR):**
    - Employ ISR with a 30-second revalidation interval to update static pages incrementally, ensuring real-time data updates without compromising performance or scalability, thereby providing up-to-date information on gadgets availability and specifications.
4. **Server-Side Rendering (SSR):**
    - Implement SSR to render dynamic content on the server, enhancing SEO capabilities and improving initial page load times for enhanced user experience, particularly for electronic gadgets details and comparisons.
5. **UI/UX Enhancements:**
    - Enhance the user interface with visually appealing components, intuitive navigation elements, and responsive design tailored to electronic gadgets enthusiasts' preferences, ensuring seamless browsing and exploration within the electronic gadgets niche.
6. **Server Components:**
    - Integrate server components to optimize rendering performance and facilitate efficient data fetching, ensuring a smooth user experience across different pages, especially for detailed gadget specifications and comparisons.
7. **Loading and Not Found Page:**
    - Design loading indicators to provide visual feedback during data fetching processes, enhancing user perception of responsiveness, and create a custom 404 (Not Found) page to gracefully handle invalid routes, guiding users back to relevant electronic gadgets listings.

# **Pages:**

## **Landing Page / Home Page: (”/”)**

*Showcase featured electronic gadgets and promotions to capture user attention and encourage exploration within the electronic gadgets niche.*

1. **Navbar:**
    - Implement a navigation bar for easy access to different sections of the website, enhancing user navigation specifically for electronic gadgets categories and brands.
    - Navbar should contain :
        - Home
        - Categories
        - Products
        - Flash Sale
        - About Us
        - Contact Us
2. **Hero Section - Carousel with Product Image:**
    - Introduce a visually engaging hero section with a carousel showcasing key electronic gadgets or promotions, enhancing aesthetic appeal and attracting electronic gadgets enthusiasts. (You can use either static images or dynamic images for carousel)
3. **Flash Sale:** 
    - Implement **ISR** with a 30s revalidation.
    - Display top 4-6 flash sale electronic gadgets, sorting based on product creation time, to highlight limited-time offers and encourage immediate purchase among electronic gadgets enthusiasts.
    - Each Product will have a flashSale property which will be a boolean value. On the basis of this value, flash sale products will be shown.
    - Provide a **"See All"** button to direct electronic gadgets enthusiasts to the **Flash Sale Products page (”/flash-sale”)** for comprehensive listings and details of discounted gadgets.
4. **Brands / Category:**
    - Show any random 6 Brands / Categories
    - Selecting brand / category depends on the niche of your project. You can either use brands or categories. For example, if your project is on mobile gadgets, you can use brands like Apple Samsung etc. If your project is based on Monitors, you can use categories like LCD, LED, AMOLED, OLED, QLED etc,
    - You can use static data to create brand / categories
    - Make sure the static data of the brands / categories are available in your products data
    - Showcase top electronic gadgets brands or categories, allowing users to explore gadgets based on their preferences and interests within the electronic gadgets niche.
    - Enable electronic gadgets enthusiasts to access a dedicated page featuring all brands or categories for extensive browsing and selection within the electronic gadgets niche.
    - Clicking a Brand / Category will navigate to **All Products Page** with filtered data of that brand. **Example :** *(“/mobiles?brand=samsung”) or (“/monitors?category=oled”)*
    - The route name for **All Products Page** will be dynamic depending on your niche. For example if your niche is mobile gadgets , your route name for All Products page will be “/mobiles”, “/gadgets” or “/electronics”.
    - Use this query parameter to filter products on the basis of brand or category in the **All Products Page**
5. **Trending Products:**
    - Implement **ISR** with a 30s revalidation.
    - Show 6 Top Rated Products based on the ratings of your products
    - Display trending electronic gadgets sorted by ratings to showcase popular items and facilitate user discovery within the electronic gadgets niche.
    - Highlight top-rated electronic gadgets and provide a **"See All Products"** button for users to explore the complete product catalog, facilitating informed purchasing decisions.
6. **Footer:**
    - Include a clickable footer section with navigation links to essential pages such as
        - Trending Products
        - Categories/Brands
        - About Us
        - Contact Us
        - Customer Care

## **Flash Sale Products Page: (”/flash-sale”) [SSR]**

- Implement **Server-Side Rendering (SSR)**
- Present all flash sale electronic gadgets with a countdown timer indicating the time remaining for each offer, fostering a sense of urgency and driving conversions among electronic gadgets enthusiasts.
- Implement a countdown timer on this page which will show the end time of the flash sale
- Countdown timer can be any time in minutes which will be dynamically / statically set.

## **All Products Page: (”/products”) [SSR]**

- The route name for All Products Page will be dynamic depending on your niche. For example if your niche is mobile gadgets , your route name for All Products page will be **“/mobiles”, “/gadgets” or “/electronics”.**
- Implement filtering options based on rating, brand/category, and price range to streamline electronic gadgets, enhancing user experience and satisfaction.

## **Single Product’s Detail Page: (”/products/:productId”) [SSR + SSG]**

- The route name for All Products Page will be dynamic depending on your niche. For example if your niche is mobile gadgets , your route name for Products Details page will be **“/mobiles/789”, “/gadgets/123” or “/electronics/456”.**
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
    - Provide a table view of all electronic gadgets for easy management and navigation, tailored specifically for electronic gadgets listings.

# **Additional Information:**

1. **Code Implementation:**
    - Utilize Next.js with Typescript for efficient file-based routing and server-side rendering and optimizing performance specifically for electronic gadgets listings.
    - Implement NextJS Data Fetching technology ensuring a robust data flow  tailored specifically for electronic gadgets browsing and comparison.
2. **Database Management:**
    - Choose MongoDB as the backend database, leveraging their capabilities for efficient data storage and retrieval.
    - Optionally, integrate Mongoose for defining database schemas and interacting with the database.
    - You can create a simple single page backend with Javascript.
3. **Improved UI/UX Design:**
    - Enhance the existing UI with responsive design, intuitive navigation, and visually appealing components tailored to electronic gadgets enthusiasts' preferences, ensuring seamless browsing and exploration within the electronic gadgets niche.
4. **Deployment:**
    - Deploy the application to a suitable hosting platform such as Vercel, [cyclic.sh](http://cyclic.sh) or any ensuring accessibility and scalability specifically for electronic gadgets listings and comparisons.

### **Submission Guidelines:**

- Include a README file in both frontend and backend repositories explaining how to set up and use the application specifically for the Electronic Gadgets Shop project.
- Provide the GitHub repository links for the frontend and backend, along with clear instructions for running the application locally, focusing specifically on electronic gadgets functionalities.
- Submit a live deployment link for the frontend application tailored specifically for electronic gadgets enthusiasts to facilitate evaluation.

### **Deadline:**

- 60 marks: March 24, 2024 11.59 PM
- 50 marks: March 25, 2024 11.59 PM
- No 30 Marks Deadline

### **Important Note:**

Plagiarism will not be tolerated. Ensure that the code you submit is your own work, tailored specifically for the Electronic Gadgets Shop project. Any instances of plagiarism will result in 0 marks.

We wish you success with your assignment! Should you have any questions or require clarification, feel free to reach out for assistance.
