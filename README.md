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
