# Use OpenJDK 21 base image
FROM eclipse-temurin:21-jdk-alpine

# Set environment variable
ENV SPRING_OUTPUT_ANSI_ENABLED=ALWAYS \
    JAVA_OPTS=""

# Set working directory
WORKDIR /app

# Copy the jar file
COPY target/url-shortener-0.0.1-SNAPSHOT.jar app.jar

# Run the jar file
ENTRYPOINT ["sh", "-c", "java $JAVA_OPTS -jar app.jar"]
