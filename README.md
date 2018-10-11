# FlyGo_Maven_Nexus3
文档地址：https://www.flygo520.com/docs/maven/maven-1an1jq32d71ge

修改工程中的 `pom.xml` 配置文件，填写你的私服地址。

<distributionManagement>
  <repository>
    <!-- 对应Maven setting.xml配置文件中 server 一一对应 -->
    <id>nexus-releases</id>
    <name>Nexus Release Repository</name>
    <url>http://${你的私服地址}/repository/flygo-hosted-releases/</url>
  </repository>
  <snapshotRepository>
    <!-- 对应Maven setting.xml配置文件中 server 一一对应 -->
    <id>nexus-snapshots</id>
    <name>Nexus snapshot Repository</name>
    <url>http://${你的私服地址}/repository/flygo-hosted-snapshots/</url>
    </snapshotRepository>
</distributionManagement>

