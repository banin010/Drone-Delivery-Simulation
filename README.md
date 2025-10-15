# Drone-Delivery-Simulation

Drone simulation project completed in the UMN software engineering course. Completed in collaboration with 3 other students, following SCRUM methodologies, facilitated through JIRA.

## 🐳 Run with Docker

You can pull and run the image directly from Docker Hub:

```bash
docker pull banin010/drone_sim:latest
docker run -it --rm -p 8080:8080 banin010/drone_sim
```

After running these commands in terminal, connect to http://localhost:8080 via your browser.

## This project contains multiple extensions made and integrated after completion

### ATC control

- Collision avoidance of drones using dot products to calculate if their paths intersect within a certain distance
- ATC uses the singleton and observer design pattern
- ATC notifies flying entities to reroute

### Drone Charging Station

- Drones have battery and automatically seek the drone charging station when out of charge

### Auditing File

- After a simulation is completed, and audit file is generated
- This file includes infromation from other extensions such as the amount of reroutes made by the ATC on each flying entity

### Drone Coordination

- When a drone needs to recharge, another drone can retrieve its package and take its place.
