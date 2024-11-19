# HomeStay: A Stay Rental Platform

**HomeStay** is a full-stack stay rental platform designed with a responsive frontend and a robust backend. It allows users to search for stays, make reservations, and manage their bookings. Built using React and Spring Boot, the platform leverages modern technologies for a seamless user experience and efficient data handling.

---

## Features
- **Frontend**:
  - Built with React and styled using Ant Design for responsive UI components.
  - Frontend hosted using npm to serve the code for browsers.
- **Backend**:
  - Developed using Spring Boot for core functionalities such as uploading stays, deleting listings, searching, and managing reservations.
  - Secured with token-based authentication using Spring Security.
- **Database**:
  - PostgreSQL integrated for stay and reservation data management.
  - Geo-based location search supported by PostGIS for enhanced search capabilities.
- **Media Management**:
  - Google Cloud Storage used for efficient handling of media file uploads (e.g., stay images).
- **Deployment**:
  - Backend services deployed on Google Cloud Run for scalable and reliable performance.

---

## Project Setup

### Frontend
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/zz9fs/HomeStay.git
   cd HomeStay/frontend
2. **Install Dependencies**:
  ```bash
  npm install
3. **Start the Frontend Server**:
  ```bash
  npm start

### Backend
1. **Clone the Repository**:
  ```bash
  git clone https://github.com/zz9fs/HomeStay.git
  cd HomeStay/backend
2. **Add Dependencies**: Use Spring Initializr to add required dependencies, or manage them in pom.xml using Maven.
3. **Configure application.yml**:
Set max-file-size to handle large uploads.
Configure rate limiting to avoid 429 Too Many Requests.
Use default-property-inclusion: non-null to optimize storage by excluding null values.
4. **Run Docker Compose**: Create and configure docker-compose.yml to set up required services.

### Database
- **Why PostgreSQL?**
  - Advanced JSON Support: Suitable for storing object-like data.
  - Location Search: PostGIS extension enables geo-indexing for faster location-based queries.
  - Array Support: Useful for handling arrays, such as image URLs.


### Additional Notes
- **Database and ORM**:
  - Spring Data Hibernate automatically generates schemas based on entity definitions.
  - Binary files like images are stored as URLs in the database for performance optimization.
- **DTO**:
  - Data Transfer Objects are used to control data access between different entities.
- **Google Cloud Services**:
  - Storage Bucket: ziang-zhang-staybooking
  - Geocoding API Key: Replace in application.yml as necessary.
