# mini-nodejs-solo-project

> Built as part of Scrimba's Node.js course.

A simple Node.js REST API serving a curated dataset of the world's most fascinating and unusual destinations, with filtering by continent, country, and public access.

## Features

- Get all destinations
- Filter by continent and/or country (query params)
- Filter by public access status
- Filter by continent or country (path params)

## Tech Stack

- Node.js (built-in `http` module, no external dependencies)

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) installed on your machine

### Installation

```bash
git clone https://github.com/nisanurcalik/mini-nodejs-solo-project.git
cd mini-nodejs-solo-project
```

### Running the server

```bash
npm start
```

The server will start on `http://localhost:8000`.

## API Endpoints

| Method | Endpoint                    | Description                          |
|--------|------------------------------|---------------------------------------|
| GET    | `/api`                       | Get all destinations                  |
| GET    | `/api?continent=Asia`        | Filter by continent (query param)     |
| GET    | `/api?country=Turkey`        | Filter by country (query param)       |
| GET    | `/api?is_open_to_public=true`| Filter by public access               |
| GET    | `/api/continent/Asia`        | Filter by continent (path param)      |
| GET    | `/api/country/Turkey`        | Filter by country (path param)        |

## Project Structure

```
├── server.js
├── data/
│   └── data.js
├── database/
│   └── db.js
└── utils/
    ├── sendJSONResponse.js
    ├── getDataByPathParams.js
    └── getDataByQueryParams.js
```

## License

ISC
