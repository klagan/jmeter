# Getting started

```bash
sudo apt-get update -y
sudo apt-get install openjdk-8-jre

JMETER_VERSION="5.4.1"
JMETER_HOME="/opt/apache-jmeter-${JMETER_VERSION}"
JMETER_BIN="${JMETER_HOME}/bin"
MIRROR_HOST="https://apache.mirrors.nublue.co.uk"
JMETER_DOWNLOAD_URL="${MIRROR_HOST}/jmeter/binaries/apache-jmeter-${JMETER_VERSION}.tgz"
JMETER_PLUGINS_DOWNLOAD_URL="http://repo1.maven.org/maven2/kg/apc"
JMETER_PLUGINS_FOLDER="${JMETER_HOME}/lib/ext/"
JMETER_DOWNLOAD_DESTINATION="/tmp/jmeter/apache-jmeter-${JMETER_VERSION}.tgz"
curl -L --silent ${JMETER_DOWNLOAD_URL} > ${JMETER_DOWNLOAD_DESTINATION}
mkdir -p /opt
tar -xzf ${JMETER_DOWNLOAD_DESTINATION} -C /opt
rm -rf /tmp/jmeter
echo "Add ${JMETER_BIN} to the PATH"

# echo $JMETER_VERSION
# echo $JMETER_HOME
# echo $JMETER_BIN
# echo $MIRROR_HOST
# echo $JMETER_DOWNLOAD_URL
# echo $JMETER_PLUGINS_DOWNLOAD_URL
# echo $JMETER_PLUGINS_FOLDER
```

---

## Sources

- [Microsoft authentication protocols](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc)
- [Cloud breaker](https://cloudbreaker.home.blog/2019/05/09/jmeter-load-testing-oauth2-secured-rest-service/)