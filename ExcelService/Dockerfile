FROM openjdk:11
ADD target/reporting.jar reporting.jar
ENTRYPOINT ["java", "-jar", "/reporting.jar"]

HEALTHCHECK --interval=10s --timeout=3s CMD curl -f http://localhost:8889/health || exit 1
