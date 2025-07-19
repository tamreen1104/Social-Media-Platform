# Social-Media-Platform
*COMPANY - CODEALPHA
*NAME - TAMREEN KHANAM
*STUDENT ID - CA/JU1/26706
*DOMAIN - FULL STACK DEVELOPMENT
*DURATION - 1st JULY 2025-30th JULY 2025
# Description
"Social Media Platform," is a foundational challenge designed to immerse interns in full-stack web development by building a miniature social media application. This project requires integrating frontend user interfaces with robust backend logic and efficient database management, mirroring the core mechanics of popular social networks. It serves as a practical exercise in creating interactive, data-driven web applications from the ground up.

Core Features to Implement:

User Profiles:
A central element of any social platform, user profiles establish individual identities within the application. For this task, each user must possess a distinct profile, which should encompass:

Username and User ID: Unique identifiers for each user, essential for both display and backend operations.

Basic Information: While not explicitly detailed, a profile typically includes a space for a user's name or a brief bio, and a visual representation like a profile picture (even if a simple placeholder).

Engagement Metrics: Crucially, profiles must display dynamic counts for the number of users who are "following" them and the number of users they are "following."

Personal Content Display: A dedicated section on the profile page should showcase all posts created by that specific user, offering a consolidated view of their contributions.

Implementing user profiles necessitates a robust user authentication system, allowing individuals to register, log in securely, and maintain persistent sessions. This ensures that profile data is managed securely and accessed appropriately.

Posts & Comments:
This feature enables content creation and user interaction, which are vital for a dynamic social platform:

Post Creation: Users must be able to compose and publish new text-based posts. Each post should be associated with its author (via user ID and username), include the content itself, and be timestamped. It should also initialize counts for likes and comments.

Content Feed: A primary "feed" or "timeline" view is required to display posts from various users. These posts should typically be presented in reverse chronological order (newest first) to keep the content fresh and relevant.

Commenting System: Users need the ability to add comments to any existing post. Each comment must be linked to its parent post, include the commenting user's ID and username, the comment's content, and a timestamp. Comments should be displayed beneath their respective posts, usually in chronological order, and the total comment count for each post must be maintained and displayed.

This aspect of the task emphasizes handling data relationships (e.g., a comment belonging to a post, a post belonging to a user) and the efficient retrieval and rendering of dynamic content.

Like/Follow System:
To foster user engagement and community building, the application must include:

Like Functionality: Users should be able to "like" a post to express approval. This action should be toggleable (liking and unliking). The system must accurately track which users have liked specific posts and display a real-time count of likes for each post.

Follow Functionality: This allows users to subscribe to the content stream of other users. When User A "follows" User B, User A indicates interest in User B's content. The system needs to manage these one-way follow relationships, updating the "followers" and "following" counts on user profiles accordingly. While a full feed aggregation based on follows isn't explicitly required for a "mini" app, the core relationship tracking is essential.

Technology Stack:

Frontend: HTML, CSS, JavaScript
The client-side interface will be built using the fundamental web trio:

HTML: Structures the application's content, defining all elements from navigation bars to post cards and comment sections.

CSS: Styles the application, ensuring a clean, intuitive, and responsive design that adapts well to various screen sizes. Modern approaches like Tailwind CSS can be utilized for efficient styling.

JavaScript: Provides the interactivity and dynamic behavior. This includes handling user authentication, making API calls to the backend, dynamically rendering and updating content on the page, and managing all user interactions (e.g., liking, commenting, following).

Backend: Django (Python) or Express.js (Node.js)
The server-side component will manage data, business logic, and expose APIs for the frontend:

Django: A robust Python web framework, offering an ORM for database interaction, built-in authentication, and a structured approach to development.

Express.js: A minimalist and flexible Node.js framework, ideal for building RESTful APIs rapidly.

Both frameworks will be responsible for defining API endpoints for all CRUD (Create, Read, Update, Delete) operations related to users, posts, comments, likes, and follow relationships. They will also handle user authentication and authorization, ensuring data integrity and security.

Database:
A persistent data store is critical for the application's functionality. The database will store:

User Data: User profiles, credentials, and associated metadata.

Post Data: Content, author, timestamps, and aggregated likes/comments.

Comment Data: Comment text, author, timestamp, and linkage to specific posts.

Relationship Data: Records for likes (who liked what) and follow relationships (who follows whom).

The database choice (e.g., SQL or NoSQL like Firebase Firestore, as demonstrated in the example) will depend on the backend framework and specific project needs, but its core role is to efficiently store and retrieve all interconnected application data.
