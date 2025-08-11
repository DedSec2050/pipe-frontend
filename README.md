# pipe-frontend

## Jenkins Integration

This project uses Jenkins for continuous integration and deployment. The Jenkins pipeline is defined in the `JenkinsFile` at the root of the repository.

### Jenkins Pipeline Overview

- **Build and Test:** The pipeline installs dependencies and runs tests using the commands defined in `package.json`.
- **Deployment:** After successful tests, the application can be deployed to the target environment.

### How to Use Jenkins with This Project

1. **Configure Jenkins:**
   - Set up a Jenkins job (Pipeline type) pointing to this repository.
   - Ensure Jenkins has access to the repository and the necessary credentials.
2. **Pipeline Script:**
   - Jenkins will automatically detect and use the `JenkinsFile` for pipeline instructions.
3. **Environment Variables:**
   - Configure any required environment variables in Jenkins or within the pipeline script.
4. **Build Triggers:**
   - Set up triggers (e.g., on push to master) as needed in Jenkins job configuration.

For more details, see the `JenkinsFile` in the root directory.
