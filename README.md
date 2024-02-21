# StudyNotion

StudyNotion is a cutting-edge educational platform designed to facilitate seamless learning experiences for students and empower instructors to showcase their expertise. Utilizing the MERN stack, StudyNotion integrates ReactJS, NodeJS, MongoDB, and ExpressJS to offer a comprehensive suite of features and functionalities.

## Key Features

- **Interactive Learning:** Engage in immersive learning experiences through StudyNotion's intuitive user interface.
- **Instructor Showcase:** Provide a platform for instructors to share knowledge and connect with learners worldwide.
- **Course Management:** Easily create, edit, and delete courses to tailor content to specific needs.
- **User Authentication:** Secure user authentication with OTP verification and password recovery functionality.
- **Payment Integration:** Seamlessly handle payments with Razorpay integration for course enrollments.
- **Media Management:** Utilize Cloudinary for efficient storage and management of media content.
- **Markdown Formatting:** Enhance course content readability with Markdown formatting.

## System Architecture

StudyNotion adopts a client-server architecture:
- **Front End:** Developed using ReactJS to deliver dynamic and responsive user interfaces.
- **Back End:** Powered by NodeJS and ExpressJS, providing robust APIs for user authentication, course management, and payment processing.
- **Database:** MongoDB serves as the primary database, storing course content, user data, and platform information.

**User Interface:**
- **Students:**
  - **Homepage:** Offers a welcoming introduction to the platform, providing quick access to the course list and user profile.
  - **Course List:** Presents an extensive catalog of available courses, complete with detailed descriptions and user ratings.
  - **Wishlist:** Conveniently showcases courses that students have earmarked for future reference.
  - **Cart Checkout:** Streamlines the process for purchasing courses, ensuring a seamless experience.
  - **Course Content:** Delivers comprehensive course materials, including videos and supplementary resources.
  - **User Details:** Displays essential account information, such as name, email, and preferences.
  - **User Edit Details:** Empowers students to customize and manage their account settings.
- **Instructors:**
  - **Dashboard:** Offers instructors an overview of their courses, along with performance metrics and learner feedback.
  - **Insights:** Provides detailed analytics on course engagement, highlighting views, clicks, and other relevant data.
  - **Course Management Pages:** Enables instructors to effortlessly create, update, and remove courses, while also managing content and pricing.
  - **View and Edit Profile Details:** Allows instructors to view and modify their profile information, ensuring accuracy and relevance.
- **Admin (Future Scope):**
  - **Dashboard:** Grants administrators visibility into platform-wide metrics, including course popularity, instructor performance, and user engagement.
  - **Insights:** Furnishes comprehensive insights into key performance indicators, such as user registrations, course enrollments, and revenue generation.
  - **Instructor Management:** Equips admins with tools to oversee instructor accounts, including user details, course listings, and performance evaluations.
  - **Other Relevant Pages:** Provides access to additional administrative functionalities, such as user management and course administration.

**Front-end Development:**
Utilizing frameworks like ReactJS, along with styling frameworks such as CSS and Tailwind, StudyNotion crafts a visually appealing and responsive user interface. Redux serves as the state management library, ensuring efficient handling of application state.

**Back-end Architecture:**
StudyNotion adopts a monolithic architecture, leveraging Node.js and Express.js for the backend, with MongoDB serving as the primary database.

**Key Features and Functionalities:**
- **User Authentication and Authorization:** Enables secure access for students and instructors, supporting features like OTP verification and password reset functionality.
- **Course Management:** Empowers instructors to create, manage, and curate courses, while students can explore, enroll, and provide feedback.
- **Payment Integration:** Facilitates seamless transaction processing through Razorpay integration, ensuring hassle-free course enrollment.
- **Cloud-based Media Management:** Harnesses the power of Cloudinary for efficient storage and management of multimedia content.
- **Markdown Formatting:** Optimizes course content for display and rendering on the frontend through Markdown formatting.

**Frameworks, Libraries, and Tools:**
- **Node.js:** Powers the backend infrastructure, providing a robust and scalable framework for application development.
- **MongoDB:** Serves as the database of choice, offering flexibility and scalability for data storage needs.
- **Express.js:** Facilitates rapid development of web applications, providing a rich set of features and tools.
- **JWT (JSON Web Tokens):** Ensures secure authentication and authorization, safeguarding user credentials.
- **Bcrypt:** Enhances security by encrypting and hashing passwords, safeguarding sensitive user data.
- **Mongoose:** Simplifies interaction with MongoDB through an intuitive Object Data Modeling (ODM) library.

**Data Models and Database Schema:**
- **Student Schema:** Includes fields such as name, email, password, and course details for each student.
- **Instructor Schema:** Consists of attributes like name, email, password, and course details for each instructor.
- **Course Schema:** Encompasses course-related information like name, description, instructor details, and media content.

## API Design

StudyNotion's API adheres to the REST architectural style and is built using Node.js and Express.js. It facilitates data exchange in JSON format and supports standard HTTP request methods like GET, POST, PUT, and DELETE. Below is a sample list of API endpoints along with their functionalities:

1. **/api/auth/signup (POST)**: Create a new user account (student or instructor).
2. **/api/auth/login (POST)**: Log in using existing credentials and generate a JWT token.
3. **/api/auth/verify-otp (POST)**: Verify the OTP sent to the user's registered email.
4. **/api/auth/forgot-password (POST)**: Send an email with a password reset link to the registered email.
5. **/api/courses (GET)**: Retrieve a list of all available courses.
6. **/api/courses/:id (GET)**: Fetch details of a specific course by its ID.
7. **/api/courses (POST)**: Create a new course.
8. **/api/courses/:id (PUT)**: Update an existing course by its ID.
9. **/api/courses/:id (DELETE)**: Delete a course by its ID.
10. **/api/courses/:id/rate (POST)**: Add a rating (out of 5) to a course.

Sample API requests and responses:

- **GET /api/courses**: 
  - Response: A list of all courses in the database.
  
- **GET /api/courses/:id**: 
  - Response: Details of the course with the specified ID.

- **POST /api/courses**: 
  - Request: Course details in the request body.
  - Response: The newly created course.

- **PUT /api/courses/:id**: 
  - Request: Updated course details in the request body.
  - Response: The updated course.

- **DELETE /api/courses/:id**: 
  - Response: A success message indicating that the course has been deleted.

## Contribution Guidelines

Contributions to StudyNotion are encouraged! Follow these steps:
1. Fork the repository.
2. Clone your forked repository to your local machine.
3. Create a new branch for your feature (`git checkout -b feature/YourFeature`).
4. Implement changes and ensure thorough testing.
5. Commit your changes (`git commit -am "Add your feature"`).
6. Push to the branch (`git push origin feature/YourFeature`).
7. Create a new Pull Request to merge your changes into the main branch.

## License

This project is licensed under the [MIT License](LICENSE).