# Snake Game Spring Boot Project

This project serves a simple, single-file Snake game from the Spring Boot static resources.

Run Application
---------------
Run with Maven (development):

```bash
mvn spring-boot:run
```

Build jar:

```bash
mvn clean package
java -jar target/snakegame-0.0.1-SNAPSHOT.jar
```

Docker
------
Build and run using Docker:

```bash
docker build -t snakegame .
docker run -d -p 8084:8084 snakegame
```

Play
----
- Open a browser at: http://localhost:8084/
- Controls: Arrow keys to move; Space to start/pause. On-screen touch buttons are available for mobile.
- Buttons: Start, Pause/Resume, Restart.

High Score
----------
High score is persisted locally in your browser using `localStorage` and displayed in the UI.

Changed files
-------------
- [src/main/resources/static/index.html](src/main/resources/static/index.html) — updated with a complete responsive Snake game

Next steps (optional)
---------------------
- Add a server-side high-score endpoint
- Add sound effects or themes
