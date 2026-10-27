# Smart India Hackathon Workshop
# Date: 26-10-2026
## Register Number: 212224040018
## Name: Ahil Santo A
## Problem Title
SIH 1710: Enhancing Navigation for Railway Station Facilities and Locations
## Problem Description
Background: Railway stations are complex environments with numerous facilities and locations such as ticket counters, platforms, restrooms, food courts, and waiting areas. Passengers often face difficulties in navigating these spaces, especially in large or unfamiliar stations. Efficient and user-friendly navigation systems are crucial for improving passenger experience, reducing congestion, and ensuring timely travel connections. Description: The problem involves developing a comprehensive navigation solution for railway stations that assists passengers in locating various facilities and destinations within the station premises. This includes creating detailed maps, providing real-time directions, and integrating features such as accessibility options for individuals with disabilities. The solution should be intuitive, easy to use, and accessible via multiple platforms, including mobile devices and digital kiosks. Key challenges include updating navigation information in real-time, ensuring accuracy, and accommodating the diverse needs of all passengers. Expected Solution: The expected solution is a multi-platform navigation system that provides detailed, real-time directions to all facilities and locations within a railway station. This system should include: A mobile application with 3D interactive maps and step-by-step navigation. Digital kiosks located throughout the station with touch-screen interfaces. Voice-guided navigation for visually impaired passengers. Regular updates to reflect changes in station layout and facility locations. Integration with existing railway apps and services for seamless user experience. The solution should enhance the overall passenger experience by reducing confusion, saving time, and improving accessibility within the station.

## Problem Creater's Organization
Ministry of Railway

## Idea

1. 3D Interactive Station Map
A multi-floor 3D map of the station showing platforms, ticket counters, restrooms, food courts, waiting halls, lifts and exits. Users can rotate, zoom, switch floors and tap any facility to see its details, timings and distance.

2. Real-Time Step-by-Step Indoor Navigation
Users pick a destination (e.g., "Platform 5" or "Nearest restroom") and get turn-by-turn directions with live position tracking using BLE beacons / Wi-Fi positioning, with QR-code scanning as a fallback when signal is weak. The route is recalculated automatically if the user goes off-path or a path is blocked.

3. Accessible Voice-Guided Navigation
Audio directions in multiple languages (English, Hindi, Tamil, etc.) for visually impaired passengers, with voice commands, haptic feedback and high-contrast UI. Wheelchair-friendly routes automatically prefer ramps and lifts and avoid stairs.

4. Smart Touch-Screen Digital Kiosks
Kiosks placed at entrances and concourses with a "You Are Here" map. Passengers can search a facility or train number, view the route, and scan a QR code to continue the same navigation on their phone.

5. Live Updates, Railway App Integration & Admin Dashboard
Station staff update layout changes, closures, platform changes and crowd levels from an admin dashboard, and these appear instantly on all apps and kiosks. Integration with existing railway apps (e.g., train status / PNR) shows the passenger's platform and the quickest route to it.

## Proposed Solution / Architecture Diagram
 
<img width="1638" height="886" alt="architecture_diagram" src="https://github.com/user-attachments/assets/8c9ead3b-2fef-4848-a98e-78492f6cf803" />


## Use Cases

<img width="1638" height="1067" alt="use_case_diagram" src="https://github.com/user-attachments/assets/dd62b285-6f77-4671-9778-8232a50954b7" />


## Technology Stack

Frontend: Flutter / React Native (mobile app), React.js (kiosk web UI), Three.js / Mapbox indoor maps (3D map)

Backend: Node.js with Express.js, WebSocket (Socket.io) for live updates

Database: PostgreSQL with PostGIS (maps and facilities), Redis (live status cache)

Positioning & Routing: BLE beacons, Wi-Fi positioning, QR-code anchors, A* / Dijkstra pathfinding

AI & Cloud: Google Text-to-Speech / Speech-to-Text, Translation API, AWS S3 / Cloud Storage

Authentication: Firebase Auth

Tools: Git, Postman, Docker

## Dependencies

Station Floor-Plan Digitization & Facility Data Collection: 12 days

3D Station Model & Map Asset Creation: 15 days

BLE Beacon Setup & Indoor Positioning Calibration: 10 days

Voice Navigation & Accessibility Testing: 7 days
