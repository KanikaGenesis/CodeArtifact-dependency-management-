# Secure Dependency Management with AWS CodeArtifact

This repository contains documentation and guide for securely managing project dependencies using AWS CodeArtifact. This project demonstrates how to set up a repository, connect it to Cloud9, and configure Maven to manage dependencies efficiently in a CI/CD pipeline.

## Setup Guide

1. **Create a CodeArtifact Repository**
   - Go to the AWS CodeArtifact console and create a new repository.

2. **Configure Maven Settings**
   - Create a `settings.xml` file in your project and add the necessary repository information and authentication details provided by CodeArtifact.

3. **Connect Cloud9 to CodeArtifact**
   - In Cloud9, configure the `settings.xml` to ensure Maven can access the CodeArtifact repository.

4. **Test the Connection**
   - Run Maven commands to compile your project and verify that dependencies are being fetched from CodeArtifact.
  
5. **Create IAM Policy**
   - Define an IAM policy using JSON to allow other services in the CI/CD pipeline (e.g., CodeBuild, CodePipeline) to access the CodeArtifact repository.

## Key Learnings

- **CodeArtifact:** Provides a secure, scalable repository for managing software packages.
- **settings.xml:** Configures Maven settings for repository locations and authentication.
- **Public Upstream Repository:** A central repository accessible to everyone for fetching updates.
- **Testing Connection:** Ensures Maven can compile the project and fetch dependencies from CodeArtifact.
- **IAM Policies:** Grant necessary permissions for CI/CD services to interact with CodeArtifact.

## Next Step

In the next part of this series, I will use AWS CodeBuild to build a WAR (Web Application Resource) file for the project.

## Author

Kanika Mathur  
[GitHub](https://github.com/KanikaGenesis) | [LinkedIn](https://www.linkedin.com/in/kanika-mathur-083080121/)
