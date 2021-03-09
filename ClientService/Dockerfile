FROM openjdk:11
ADD target/main.jar main.jar
ENTRYPOINT ["java", "-jar", "/main.jar"]

HEALTHCHECK --interval=10s --timeout=3s CMD curl -f http://localhost:8081/health || exit 1
