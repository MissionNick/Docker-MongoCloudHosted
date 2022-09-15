# Docker-MongoCloudHosted

Do the following to create and then allow access to containers

1. Create Google Compute Engine
    - Vanilla VM
    - Install Docker and Docker compose
2. Create docker compose file - example provided
    - Creates volumes, network, container servers
3. Upload docker compose file
4. Execute docker compose file
5. Update firewall rules to allow public access  - Apply to all targets 
    - 8081 MongoDB express
    - 27017 MondoDB (if web service is on another instance)
6. Import all dbs and documents etc.  Initialise DB. After which the volumes will keep data during docker down and up events.
7. Establish volume backups.  Docker RMI 

To do
- Cleanup anon volumes on service restart
- Tighten up security access