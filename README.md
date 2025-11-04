# pre-flight


Phase 1: Foundation & Simulation

Goal: Get the app running, visualize fake drone telemetry, and learn the stack.

Focus: Build your full-stack structure and get simulated data showing up live.

🧠 Core Features

React + TypeScript frontend with a clean dashboard (e.g. Tailwind UI)

Node.js + Express + TypeScript backend

Simulated telemetry via WebSocket or Socket.io

Basic metrics display: altitude, speed, battery, GPS coordinates

Simple JSON type sharing between frontend and backend

🧰 Tech Setup
Layer	Tech
Frontend	React + Vite + TypeScript
Backend	Node.js + Express + Socket.io
UI	Tailwind CSS or shadcn/ui
Data	Simulated generator function
Hosting (optional)	Vercel (frontend), Render (backend)
🧭 Learning Goals

TypeScript type sharing between frontend and backend

Real-time updates via WebSockets

Basic UI composition and state management

✅ Outcome:
A working web dashboard that shows simulated drone data updating in real-time.

🧱 Phase 2: Intermediate — Visualization & Multi-Drone

Goal: Move beyond mock data to richer simulation and visualization.

Focus: Add maps, multiple drones, and better architecture.

🧠 Core Features

Map view with drone markers (Leaflet.js or Mapbox)

Simulate multiple drones (array of telemetry data)

Smooth real-time position updates and paths

Modular data layers (telemetry provider, socket listener)

Custom drone icons and tooltips (altitude, speed, battery)

🧰 Tech Setup
Layer	Tech
Maps	Leaflet.js + OpenStreetMap tiles
State	React Context or Zustand
Data model	Type-safe telemetry interfaces
Optional	Chart.js or Recharts for graphs
🧭 Learning Goals

Integrating external libraries (Leaflet, charts)

Managing complex state

Designing reusable, strongly typed components

✅ Outcome:
An interactive multi-drone dashboard — users can view, switch, or filter drones in real-time.

🛰️ Phase 3: Real Hardware & Control

Goal: Replace simulated data with actual telemetry from a drone.

Focus: Integrate a real drone SDK or API (like DJI or Tello).

🧠 Core Features

Connect backend to drone via SDK or UDP

Stream live telemetry to the frontend

Add basic command buttons (takeoff, land, hover)

Create a simple safety mechanism (confirm commands)

Store telemetry logs locally (JSON or SQLite)

🧰 Tech Setup
Layer	Tech
Drone	Tello SDK / DJI SDK
Protocol	UDP or WebSocket
Storage	SQLite or JSON file
Command flow	Express route → socket event → SDK command
🧭 Learning Goals

Hardware integration

Network data parsing (e.g., UDP packets)

Safe command and telemetry flow

✅ Outcome:
A fully working web-based drone control and telemetry viewer with real data.

⚙️ Phase 4: Advanced Intermediate — Persistence & Cloud

Goal: Store and analyze flight data; add authentication for multiple users.

Focus: Turn the project into a lightweight, cloud-deployed app.

🧠 Core Features

Store flight logs (in PostgreSQL or Supabase)

Add authentication (Firebase or Auth0)

Save and replay past flights

Deploy backend + frontend publicly (Render + Vercel)

Cloud database for user data and telemetry logs

🧰 Tech Setup
Layer	Tech
Database	PostgreSQL / Supabase
Auth	Firebase Auth / Auth0
Hosting	Render (backend), Vercel (frontend)
Deployment pipeline	GitHub Actions (optional)
🧭 Learning Goals

Connecting to cloud services

Structuring REST APIs and WebSocket streams together

Managing users, tokens, and secure data storage

✅ Outcome:
FlightCTRL v2 — a polished, multi-user drone dashboard that logs flights, saves telemetry, and streams live control data securely.

🧪 Optional Phase 5: Exploration

Goal: Make it cutting-edge and fun to show off.

🚀 Add-On Ideas

AI-assisted flight predictions (using TensorFlow.js or a small ML model)

Path drawing → send flight path commands to drone

3D visualization (using Three.js or Cesium)

Mobile companion app (React Native)

Voice or gesture-based control input

✅ Outcome:
A showcase-level project that impresses employers, schools, or hackathons — professional, technical, and creative.
