# CompDoku

CompDoku is a competitive Sudoku web application that allows users to practice or compete against other players in real time.

Live site: https://compdoku.com

## Overview

CompDoku was built as an exploration into web development. The goal was to gain hands on experience building and deploying a full stack application while strengthening C++ skills.

The application supports:

- Practice mode via REST API  
- Competitive mode via WebSocket connections  
- Real time win and loss enforcement on disconnect  

## Architecture

### Frontend

- Vite  
- TypeScript  
- Tailwind CSS  

The frontend handles board rendering, user interaction, and communication with the backend APIs and WebSocket server.

### Backend

- C++  
- Crow  
- SQLite  

The backend provides:

- REST endpoints for generating practice boards and solutions  
- WebSocket connections for competitive multiplayer matches  
- Game state validation and win detection  
- Disconnect detection to award wins automatically  

Sudoku generation and validation logic is implemented in C++.

## Deployment

- Hosted on Oracle Cloud Always Free tier  
- NGINX used for static file serving and reverse proxy  
- NGINX routes frontend traffic and proxies API and WebSocket requests to the backend  

## Future Improvements

- User authentication  
- Leaderboards  
- Multiple difficulty levels  
- Persistent match history  

