# Metro Tracker

A real-time 3D visualization of the New York City subway system built with Next.js, Three.js, and the MTA's real-time data feed.

![Screenshot 2025-01-12 150500](https://github.com/user-attachments/assets/dcb6f3ae-3b3c-456f-8eb0-a3bba833315b)


## Features

- Real-time subway train positions
- 3D visualization of the NYC subway system
- Interactive camera controls
- Live updates from MTA's GTFS feed
- Beautiful 3D rendering with Three.js
- Responsive design

## Prerequisites

Before you begin, ensure you have the following installed:
- [Node.js](https://nodejs.org/) (v20 or later)
- [Docker](https://www.docker.com/) (optional, for containerized deployment)
- An MTA API key (get one from [MTA's Real-Time Data Feeds](https://api.mta.info/))

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/metro-tracker.git
cd metro-tracker
```

2. Install dependencies:
```bash
npm install
```

## Development

Run the development server:
```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) to view the application.

## Docker Deployment

1. Build the Docker image:
```bash
docker compose build
```

2. Run the container:
```bash
docker compose up
```

## Project Structure

```
metroapp/
├── src/
│   ├── app/                 # Next.js app directory
│   │   ├── api/            # API routes
│   │   ├── components/     # React components
│   │   ├── services/       # Service layer (MTA API)
│   │   └── page.tsx        # Main page component
│   ├── generated/          # Generated protobuf types
│   └── proto/              # Protobuf definitions
├── public/                 # Static assets
├── Dockerfile             # Docker configuration
└── docker-compose.yml    # Docker Compose configuration
```

## Technologies Used

- [Next.js](https://nextjs.org/) - React framework
- [Three.js](https://threejs.org/) - 3D graphics library
- [TypeScript](https://www.typescriptlang.org/) - Type-safe JavaScript
- [Protobuf](https://protobuf.dev/) - Data serialization
- [Docker](https://www.docker.com/) - Containerization

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
