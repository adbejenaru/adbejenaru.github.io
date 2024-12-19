# Key Contributions and Achievements as a Software Engineer at Deutsche Bank

## L3 Production Support for Trading Platform
- Acted as the primary point of contact for weekly platform issue resolutions, ensuring system reliability and minimal downtime.
- Resolved critical production incidents, including scenarios where platform components prevented the main application from running. 
  - Quickly identified root causes, implemented solutions, and applied preventative measures.

## Configured FIX Sessions for Order Types
- Set up FIX sessions tailored to support order processing, ensuring seamless communication and message handling between trading platforms and internal systems.

## Enhanced System Clean Handling
- Addressed issues where force system clean bypassed validation checks after three failed attempts during startup.
- Configured cron jobs to handle scenarios requiring force system clean (disabled for UAT, enabled for PROD), preserving the integrity of pre-clean validation checks.

## Migrated from Outdated Spring Boot with Ribbon
- Transitioned from an outdated Spring Boot version with Ribbon (incompatible with Spring Boot 3) to Spring Cloud Load Balancer for enhanced compatibility, scalability, and resilience.
- Refactored microservice configurations and dependencies to align with Spring Boot 3 standards.

## Investigated and Resolved Microservices Issues
- Debugged and resolved HTTP exceptions caused by invalid client requests to external platforms, enhancing error handling for compatibility with external APIs like Aladdin.
- Diagnosed report generation issues and implemented regex-based solutions for robust parsing of record counts and variable spacing.
- Collaborated with cross-functional teams for debugging and implemented fixes documented in the project knowledge base for future reference.

## Documentation for Fixed Income APAC Pre-Trade Check Project
- Authored comprehensive documentation and created detailed diagrams illustrating microservice interactions, request flows, FIX sessions, HTTPS connectivity, and API-proxy usage.
- Mapped microservices to respective endpoints and documented required authorizations for actions, including permissions for API-proxy interactions and FIX session integrations.
- Cataloged FIX sessions and Solace connectivity details, providing clear guidelines for developers and stakeholders.

## JMX Actions for File Generation
- Developed JMX actions to trigger trade information file generation from Swagger, enabling QA and BA testers to generate MFOUT files for functional testing.

## External Platform Order Simulator Integration
- Introduced a platform (PM1) order simulator, developing FIX producers and consumers for various order types (FI, EQ, FX, MF).
- Created JMX operations to simulate single-order and multi-order flows.

## Post-Trade Transparency (PoTT) Reporting System
- Designed and implemented a comprehensive system for MiFID2 compliance.
- Developed caching mechanisms for PoTT alerts, automated EOD CSV generation, and configured email submissions to L2 support teams.

## Email Normalization in GCP Environments
- Refactored email lookup logic to accommodate custom email domains used in GCP testing environments, ensuring compatibility with microservices still operating on legacy on-prem email formats.

## Memory Optimization for Microservices
- Configured environment-specific memory parameters for various microservices, improving resource allocation and reducing overhead.
- Enabled historical memory tracking through Prometheus and Spring Boot Actuator integration.

## ActiveConsole Geneos Alerts and Monitoring
- Streamlined alert configurations for regional distribution and replaced deprecated server configurations in ActiveConsole.

## Legacy File Archiving and Cleanup
- Investigated and resolved file visibility issues in ServerGrid by implementing archiving mechanisms for older files in weekly directories.
- Configured cleanup tools for efficient file management across INT, UAT, and PROD environments.

## GCP Image Vulnerability Mitigation
- Onboarded secure Docker images and transitioned to version-controlled YAML manifests for stable deployment.
- Performed Xray scans to ensure compliance and mitigate critical CVEs in GCP environments.
