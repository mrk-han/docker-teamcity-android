# docker-teamcity-android
TeamCity server &amp; agent containers for painless setup with Docker for Android Development.

### Setup

```bash
# full URL for TeamCity server, accessible by the agent
export SERVER_URL=http://<TEAMCITY_SERVER_URL>:8111

# optional, see: https://confluence.jetbrains.com/display/TCD10/TeamCity+Data+Directory
export DATA_PATH=<TEAMCITY_DATA_DIR>

# optional, stores TeamCity server logs
export LOGS_PATH=<TEAMCITY_LOGS_DIR>

# optional, stores TeamCity agent config
export CONF_PATH=<AGENT_CONF_DIR>

# build provided image & start docker containers
docker build -t teamcity-android-agent .
docker-compose up server agent
```
