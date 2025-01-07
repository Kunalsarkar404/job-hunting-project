Job Hunting Project
===================

This is a basic project where you can add job openings and view them. The application also provides a filter and search bar for real-time job filtering.

Features
--------

The repository contains two main components:

-   Backend service for managing job data and handling API requests.
-   Frontend service for displaying job openings and user interactions.

Technologies Used
-----------------

-   **Frontend:** React.js (Hooks, State Management)
-   **Backend:** Spring Boot (RESTful APIs, Data Management)
-   **Database:** MongoDB Atlas (NoSQL Database)
-   **Version Control:** Git

Installation
------------

1.  Clone the repository:

    ```
    git clone <repository-url>

    ```

2.  Navigate to the project directory:

    ```
    cd job-hunting-project

    ```

3.  Install frontend dependencies:

    ```
    cd frontend
    npm install

    ```

4.  Install backend dependencies:

    ```
    cd backend
    mvn clean install

    ```

5.  Set up MongoDB Atlas connection in `application.properties`:

    ```
    spring.data.mongodb.uri=mongodb+srv://<username>:<password>@cluster0.mongodb.net/<database>

    ```

Usage
-----

1.  **Start Backend:**

    ```
    cd backend
    mvn spring-boot:run

    ```

2.  **Start Frontend:**

    ```
    cd frontend
    npm start

    ```

3.  Access the app at `http://localhost:3000`.

API Endpoints
-------------

-   `GET /api/jobs` -- Fetch all job applications.
-   `POST /api/jobs` -- Add a new job application.
-   `PUT /api/jobs/{id}` -- Update a job application.
-   `DELETE /api/jobs/{id}` -- Delete a job application.

Contributing
------------

Contributions are welcome! Please follow these steps:

1.  Fork the repository.
2.  Create a new branch: `git checkout -b feature-name`
3.  Commit your changes: `git commit -m 'Add feature'`
4.  Push to the branch: `git push origin feature-name`
5.  Open a pull request.

Contact
-------

-   **Author:** Kunal Sarkar
-   **Email:** <interviewkunal@gmail.com>