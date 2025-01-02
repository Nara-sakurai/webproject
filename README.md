# Sneaker Shoe Web Project

This is a web-based project for managing sneaker shoes. The project includes functionalities to manage products (sneakers) and users. It uses a MySQL database for data storage and retrieval and implements a Node.js backend with Express.js. The project also follows the MVC (Model-View-Controller) architecture for organizing code and implementing CRUD (Create, Read, Update, Delete) operations effectively.

## Project Structure

```
webproject/
├── config/
│   ├── database.js
│   ├── multer.js
├── controllers/
│   ├── indexController.js
│   ├── productController.js
├── models/
│   ├── productModel.js
│   ├── userModel.js
├── public/
│   ├── css/
│   │   ├── image/
│   │   ├── style.css
├── routes/
│   ├── indexRoutes.js
│   ├── productRoutes.js
├── views/
│   ├── index/
│   │   ├── index.ejs
│   ├── partials/
│   │   ├── footer.ejs
│   │   ├── header.ejs
│   ├── product/
│   │   ├── create.ejs
│   │   ├── edit.ejs
│   │   ├── index.ejs
│   │   ├── show.ejs
│   ├── user/
│   │   ├── login.ejs
├── .env.sample
├── .gitignore
├── package.json
├── server.js
```

### Key Directories and Files

- **config/**: Configuration files including database setup (`database.js`) and file upload settings (`multer.js`).
- **controllers/**: Contains controller logic for handling requests and responses.
- **models/**: Contains database models for products and users.
- **public/**: Static files such as CSS and images.
- **routes/**: Routing logic for handling application endpoints.
- **views/**: EJS templates for rendering the front-end. Subdirectories include:
  - **index/**: Contains the main `index.ejs` file.
  - **partials/**: Reusable components like `footer.ejs` and `header.ejs`.
  - **product/**: Templates for managing products (`create.ejs`, `edit.ejs`, `index.ejs`, `show.ejs`).
  - **user/**: Templates for user-related actions like `login.ejs`.
- **server.js**: Entry point of the Node.js application.

---

## Features

1. **Products Management**:

   - Add, view, update, and delete sneaker products.
   - Products are stored in the `product` table within the `gproducts` database.

2. **User Management**:

   - Register and manage user accounts.
   - Users are stored in the `users` table within the `gproducts` database.

3. **Dynamic Web Pages**:

   - EJS templates for rendering dynamic content.

4. **Database Integration**:

   - MySQL database connectivity for storing and retrieving product and user data.

5. **Flash Messages**:

   - Inform users of actions (success, error, etc.) through flash messages.

6. **Image Upload**:

   - Allows uploading images for products using Multer.

7. **Delete Alerts**:

   - Confirmation alerts for deleting records.

8. **PHP Integration**:

   - PHP is used to manage and interact with the MySQL database via MAMP for database creation and testing.

9. **MVC Architecture**:

   - Implements a clear separation of concerns using the Model-View-Controller design pattern for better code organization.

10. **CRUD Operations**:

    - Provides complete CRUD functionality for managing products and users.

---

## Prerequisites

- **Node.js**: Ensure Node.js is installed.
- **MySQL**: Set up and configure a MySQL database.
- **MAMP**: If using MAMP, ensure it is configured properly.
- **PHP**: Use PHP for database management and integration testing in MAMP.

---

## Installation

1. Clone the repository:

   ```bash
   git clone <repository-url>
   cd webproject
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Set up the environment variables:

   - Copy `.env.sample` to `.env` and update the following variables:
     ```env
     DB_HOST=localhost
     DB_USER=root
     DB_PASSWORD=yourpassword
     DB_NAME=gproducts
     ```

4. Start the application:

   ```bash
   node server.js
   ```

5. Access the application at `http://localhost:3000`.

---

## Database Schema

### Products Table (`product`)

- **Columns**:
  - `id`: Primary key.
  - `name`: Name of the sneaker.
  - `description`: Description of the sneaker.
  - `price`: Price of the sneaker.
  - `image`: Path to the product image.

### Users Table (`users`)

- **Columns**:
  - `id`: Primary key.
  - `username`: Username of the user.
  - `email`: Email of the user.
  - `password`: Encrypted password.

---

## Dependencies

- **Node.js**
- **Express.js**
- **MySQL**
- **EJS**
- **Multer**
- **Flash Messages**
- **PHP**

---

## Future Enhancements

- Implement user authentication (login and registration).
- Add search functionality for products.
- Improve UI/UX design.
- Implement role-based access control.

---

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your proposed changes.

---

## License

This project is licensed under the MIT License. See the LICENSE file for details.

---

## Contact

For any questions or suggestions, feel free to reach out to the project team.

