### README FOR GEO-PUZZLE

Lately, with the advent of the GPS, people have been getting into an activity called geocaching, where people have to use
their GPS to track down specific boxes to containers that contain something inside of them. Based on that idea, I worked in a team to create Virtual-Geopuzzle, an app where one can leave video and audio files so that when someone gets to a particular location, these files start playing to let someone know where they should go next to find the next clue. This continues until the user reaches a 
particular location, and they have won the game. 
This app was created for entertainment purposes to get the user interested in playing puzzles with their friends
as use of their free time.

#### Development Environment Setup for Rails Server

Install Docker or Docker Toolbox (Device Specific)

1. **Start** Docker Quickstart Terminal

2. **Clone** the repo above

3. **Create** a `.env` file (or move .env.dev to .env)
```text
RAILS_ENV=development
WEB_DATABASE_PASSWORD=password
```

4. **Build** the `web`, and `db` containers:
```bash
docker-compose build
```

5. **Start** the `web` and `db` services
Omit the `-d` option if you want to see the output of the command, or for debugging:
```bash
docker-compose up -d
```

If your using Docker Toolbox, the website should be available at:
http://http://192.168.99.100/
Otherwise, the website should be available at:
http://localhost:80

**Stop** and **Remove** containers and networks:
```bash
docker-compose down
```

#### Development Environment Setup for React Native Application

Install React Native Cli, Java JDK, and Android SDK
Set the proper environment variables

1. **Start** Terminal of choice

2. **Clone** the repo above

4. **Go** into the `frontend` directory
```bash
cd frontend/
```

5. **Install** the node_modules
```bash
npm install
```

6. **Open** an emulator
Use an emulator so your app will be able to hit the rails server

7. **Start** the application
```bash
react-native run-android
```
