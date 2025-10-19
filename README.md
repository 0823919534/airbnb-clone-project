# airbnb-clone-project

AirBnB Clone — learning project to reproduce core features of a short-term rental marketplace.
Goals: implement user auth, property listings (CRUD), search/filter, booking flow, and a responsive UI.

## Database Design

The project uses a relational database structure to manage users, property listings, and bookings.

**Entities:**
- **User:** stores user information such as name, email, and role (guest or host)
- **Listing:** represents a property listed by a host with fields like title, description, price, and location
- **Booking:** links a guest to a listing with start and end dates, total price, and status

**Relationships:**
- A user (host) can have many listings
- A listing can have many bookings
- A user (guest) can make many bookings

The database will be managed using Sequelize ORM with SQLite in development and PostgreSQL in production.

## Technology Stack

- **React / Vite / Next.js:** Frontend libraries/frameworks for building the user interface.
- **Node.js & Express:** Backend runtime and web framework for building RESTful APIs.
- **Sequelize / ORM:** Object-Relational Mapper for interacting with the database.
- **SQLite / PostgreSQL:** Relational databases for development and production.
- **JWT / Passport.js / NextAuth:** Authentication mechanisms for secure login.
- **AWS S3:** Storage for listing images.
- **Jest / React Testing Library / Supertest:** Testing tools.
- **Docker / Docker Compose:** Containerization for consistent dev environments.
- **CI / CD (GitHub Actions, Vercel, Heroku, Railway):** Deployment automation.
- **Axios / Fetch:** Frontend HTTP clients.
- **bcrypt / jsonwebtoken:** Password hashing and token management.
- **ESLint / Prettier:** Code quality and formatting tools.

## Feature Breakdown

The AirBnB Clone project includes the following main features:

- **User Management:** Allows guests and hosts to create accounts, log in securely, and manage profiles. This feature supports authentication, authorization, and role-based access for different types of users.

- **Property Management:** Enables hosts to create, edit, and delete property listings, including details like title, description, price, and images. This feature ensures listings are well-organized and discoverable by guests.

- **Booking System:** Lets guests browse listings, select available dates, and book properties. It handles scheduling conflicts, calculates total price, and updates booking status, ensuring a smooth rental experience.

- **Search & Filtering:** Allows guests to search listings by location, price, and other criteria. This improves usability and helps users find properties that match their preferences.

- **Reviews & Ratings (optional):** Guests can leave reviews and ratings for listings they have stayed at. This helps maintain quality and trust within the platform.

- **Notifications (optional):** Sends alerts to users for booking confirmations, cancellations, and updates. This keeps users informed and engaged.

## Future Sections (placeholders)

- ## User Authentication
- ## Listings CRUD
- ## Booking Flow
- ## Deployment
