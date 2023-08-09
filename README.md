<p align="center">
  <img src="https://raw.githubusercontent.com/atulmy/atulmy.github.io/master/images/hire-smart/hero-shadow.png" alt="Hire Smart" />
</p>

<h1 align="center">Workly</h1>
<p align="center">An application for human resource team / recruitment consultancies to streamline hiring process, scheduling interviews and tracking candidates.</p>

## Technology Stack
  - API
    - Node
    - Express
    - MongoDB
    - Remote Procedure Call
    - Outlook
    - Pandas/Open libraries
  - Web
    - React
    - Redux
    - React Router
    - Material UI

## Setup and Running
- Prerequisites
  - Node
  - MongoDB
- Clone repo `git clone https://github.com/ShivamAgarwal-code/Workly.git`
- Switch to `code` directory `cd code`
- Configurations
  - API
    - Create local environment file `cp /api/.env.example /api/.env.local`
    - Modify `/api/.env.local` for database credentials
    - Modify `/api/.env.local` for PORT (optional)
  - Web
    - Create local environment file `cp /web/.env.example /web/.env.local`
    - Modify `/web/.env.local` for PORT / API URL (optional)
- Setup
  - API: Install packages and database setup (migrations and seed) `cd api` and `npm run setup`
  - Webapp: Install packages `cd web` and `npm install`
- Development
  - Run API `cd api` and `npm start`, browse at http://localhost:3000/
  - Run Webapp `cd web` and `npm start`, browse web at http://localhost:3001/
- Deployment
  - Without Docker
      - Configure nginx on server
      - Run API `cd api` and `npm run start:prod`, creates an optimized build in `build` directory and runs the server
      - Run Webapp `cd web` and `npm run start:prod`, creates an optimized build in `build` directory and runs the server
  - Using Docker
      - `cd code/deploy`
      - Update your domain, SSL certificate path and other configurations in `docker-compose.yml`
      - Start Docker containers: `docker-compose up -d`
        
  The MIT License (http://www.opensource.org/licenses/mit-license.php)
