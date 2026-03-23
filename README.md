# Apollo Remote Desktop

## Project Overview
Apollo Remote Desktop is a revolutionary remote access solution that provides low-latency, high-performance connection using cutting-edge technologies. This project allows seamless remote desktop access with superior performance, tailored for both personal and professional use.

## High-Performance Modes
### Moonlight Mode
Designed for games and real-time applications, Moonlight Mode optimizes performance with minimal latency.

### Sunshine Mode
Sunshine Mode focuses on delivering superior graphics and smooth interfaces for productivity tasks.

## Setup Instructions
### Prerequisites
Ensure you have the following installed on your machine:
1. **Node.js** (version 18 or higher)
2. **pnpm** package manager

### Detailed Setup and Installation Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/Arkhishere/Remote-Desktop.git
   cd Remote-Desktop
   ```
2. Install dependencies using pnpm:
   ```bash
   pnpm install
   ```
3. Create a `.env` file in the root of the project with the following configurations:
   ```env
   PORT=3000
   SIGNALING_PORT=8080
   SECRET_KEY=your_secret_key_here
   ```
   Replace `your_secret_key_here` with a secure key of your choice.
4. Start the application:
   ```bash
   pnpm start
   ```

## Networking and Architecture
### P2P WebRTC Handshake Mechanism
The architecture leverages a P2P WebRTC handshake mechanism to establish direct connections between clients, optimizing the data exchange for speed and efficiency.

### Networking Tips
For optimal connectivity, ensure the following ports are open:
- **TCP**: 3000, 8080  
- **UDP**: 47998-48010

For users behind strict NATs or firewalls, consider using VPN tunnels like **Tailscale** to facilitate connectivity.

## Contributing
We welcome contributions! Please follow these guidelines:
1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Submit a pull request with a detailed description of your changes.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.