# Rent and Go (Backend)

Backend for [Rent and Go](https://github.com/rmirandasv/rent-and-go) powered by [Strapi](https://strapi.io).  

Rent and Go is an open-source car rental web application with a Strapi backend and Next.js frontend.

## Key Features
- Manage brands, car models, vehicles, and rental requests from customers.
- Google Sign-In for user authentication.
- User dashboard to manage rental requests and preferences.

## Installation

### Prerequisites
Make sure you have the following installed on your system:
- [Node.js](https://nodejs.org/) (v16 or higher is recommended)
- [npm](https://www.npmjs.com/) or [yarn](https://yarnpkg.com/)

### Steps

1. Clone this repository:
   ```bash
   git clone https://github.com/rmirandasv/rent-and-go-backend.git
   cd rent-and-go-backend
   ```

2. Install dependencies:
   ```bash
   npm install
   # or
   yarn install
   ```

3. Start the development server:
   ```bash
   npm run develop
   # or
   yarn develop
   ```

   The backend will be available at [http://localhost:1337](http://localhost:1337).

### Environment Variables

Create a `.env` file in the root directory and configure the following variables:

```env
# Server
HOST=0.0.0.0
PORT=1337

# Secrets
APP_KEYS=
API_TOKEN_SALT=
ADMIN_JWT_SECRET=
TRANSFER_TOKEN_SALT=

# Database
DATABASE_CLIENT=sqlite
DATABASE_HOST=
DATABASE_PORT=
DATABASE_NAME=
DATABASE_USERNAME=
DATABASE_PASSWORD=
DATABASE_SSL=false
DATABASE_FILENAME=./route-ro-you-db.sqlite
JWT_SECRET=
```  

For advanced configurations, see the [Strapi Environment Configuration Guide](https://docs.strapi.io/dev-docs/configurations).

## Database Configuration

By default, this application uses SQLite for the database. You can configure a different database (e.g., PostgreSQL, MySQL) by following these steps:

1. Install the database package:
   ```bash
   npm install pg   # For PostgreSQL
   npm install mysql # For MySQL
   ```

2. Update the `config/database.js` file with your database credentials. Refer to the official [Strapi Database Configuration Documentation](https://docs.strapi.io/dev-docs/configurations/database).

## Deployment

For deploying this Strapi backend, follow the [official Strapi deployment guide](https://docs.strapi.io/dev-docs/deployment). Some commonly used platforms include:
- [Heroku](https://www.heroku.com/)
- [AWS](https://aws.amazon.com/)
- [DigitalOcean](https://www.digitalocean.com/)

## Links and References

- [Rent and Go Frontend Repository](https://github.com/rmirandasv/rent-and-go)
- [Strapi Documentation](https://docs.strapi.io/)
- [Strapi Plugins Marketplace](https://market.strapi.io/)
- [Customizing Strapi API](https://docs.strapi.io/dev-docs/plugins-and-customization/routes)

---

Feel free to contribute to this project by creating issues or submitting pull requests. Happy coding!

