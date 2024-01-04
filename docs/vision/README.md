# Vision for api.ed-fi.org

This and subsidiary documents server as the initial requirements and ideation
about the deployment process. The [parent directory](../) will contain
documentation of the processes as implemented.

## Organizational Goal

Deploy the Ed-Fi ODS/API and related tools into Azure cloud services with
multiple environments:

1. **Staging**, under https://api-stg.ed-fi.org and serving as a demonstration
   of unstable (pre-release) code.
2. **Demonstration**, under https://api.ed-fi.org and serving as a full
   demonstration environment of released (stable) code.
3. **Certification**, under https://certification.ed-fi.org, and serving the
   needs of the Certification process, using released code.

In each case, the architectural components should be the same. The key
differences between these environments are the deployment triggers and the
images or packages used for the deployment.

## Tech Stack

Based on similar projects, we expect to use some or all of the following tools
and services:

1. Source code and build automation continues in GitHub.
2. Azure DevOps for deployment orchestration.
3. TerraForm for managing desired state deployments.
4. Azure Cloud services for hosting.
   1. Web hosting options:
      1. VM
      2. App Services
      3. Container App
   2. Database hosting options:
      1. VM
      2. Azure SQL
      3. Container App
   3. API Gateway
   4. Azure Monitor
      1. Application Insights
      2. Log Analytics

## Further Detail

* [Environments](./ENVIRONMENTS.md)
* [Automation](./AUTOMATION.md)
