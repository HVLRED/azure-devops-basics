# Use Apache Tomcat as the base image
FROM tomcat:latest

# Remove the default ROOT application
RUN rm -rf /usr/local/tomcat/webapps/ROOT

# Copy your WAR file to the Tomcat webapps directory
COPY webapp.war /usr/local/tomcat/webapps/ROOT.war

# Expose port 8080 to allow incoming HTTP traffic
EXPOSE 8080

# Start Apache Tomcat when the Docker container starts
CMD ["catalina.sh", "run"]
