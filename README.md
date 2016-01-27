# SpringBootNewRelicApplication

To start the application and see it report to your newrelic account:

- input your license in ``src/main/resources/newrelic.yml`` (replace ``license_key: '12345'`` with yours)
- ``mvn clean package``
- ``java -Dnewrelic.config.file=src/main/resources/newrelic.yml -javaagent:target/spring-boot-new-relic-0.0.1-SNAPSHOT.jar -jar target/spring-boot-new-relic-0.0.1-SNAPSHOT.jar``

You can then login to your newrelic account and should be able to see your app reporting.