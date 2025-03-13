# High-Speed Download Manager

A web-based download manager optimized for mobile browsers, featuring multi-threaded downloads and a modern UI.

## Features Implemented

1. **File Browser**
   - Browse files and directories
   - File search functionality
   - File metadata display (size, type, modified date)
   - Secure file access with path traversal protection

2. **Authentication System**
   - Login/logout functionality
   - Session management
   - Protected routes
   - Automatic redirect to login

3. **Modern UI**
   - Vue.js with Vuetify components
   - Mobile-responsive design
   - Dark/light theme support
   - Snackbar notifications
   - Progress indicators

4. **Real-time Updates**
   - WebSocket connection for live updates
   - Download progress tracking
   - Connection status monitoring

5. **Security Features**
   - CORS protection
   - Session-based authentication
   - Secure file access
   - Rate limiting
   - Helmet security headers

## Upcoming Features

1. **Multi-threaded Downloads**
   - Chunked download implementation
   - 2-6 threads for mobile optimization
   - Download resume capability
   - Progress tracking per chunk

2. **Download Management**
   - Pause/Resume functionality
   - Download queue
   - Download history
   - Batch operations

3. **Mobile Optimizations**
   - Touch-friendly interface
   - Offline capability
   - Add to Home Screen
   - Push notifications

## Deployment Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/weir1/high-speed-download-manager.git
   cd high-speed-download-manager
   ```

2. Install dependencies:
   ```bash
   npm install
   cd server
   npm install
   cd ..
   ```

3. Configure environment:
   ```bash
   cp server/.env.example server/.env
   ```
   Edit `server/.env` and set:
   - `PORT`: Server port (default: 5000)
   - `BASE_PATH`: Directory to serve files from
   - `SESSION_SECRET`: Secure random string
   - `CORS_ORIGIN`: Frontend URL

4. Build the application:
   ```bash
   npm run build
   cd server
   npm run build
   cd ..
   ```

5. Start the server:
   ```bash
   node start.js
   ```

## Security Notes

- Use HTTPS in production
- Set strong SESSION_SECRET
- Configure proper CORS settings
- Set appropriate file permissions

## Requirements

- Node.js 18+
- Modern web browser with WebSocket support