In this exercise I will reflect on the continuous integration of a Java-based application in a team of six people.

From my Google research, it would seem that the most used tools for linting, testing and building Java applications are Maven and Gradle with their plugins and libraries. Some example tools are Checkstyle and SonarQube for linting and JUnit and TestNG for testing. All of these can be integrated into Maven or Gradle, which will in turn take care of the building part of the process.

Besides Jenkins and GitHub Actions, there are other services for setting up the CI/CD pipeline for a Java project. Some examples for cloud-based ones that I found are CircleCI and TravisCI as well as Gitlab CI. For self-hosted options, many of the cloud-based ones seem to offer a self-hosted option as well. All of the examples I mentioned at least have the option. TeamCity seems to be a reversal of this, being a self-hosted server first and a cloud service second. Another interesting option I came across is Buildkite which is a hybrid CI/CD platform: you host your own agents while using cloud-based UI and orchestration.

As to whether this team should go for a self-hosted or a cloud-based approach, I would have to know more of the nature of the product they are making. Does it have special requirements for running tests which a cloud service might not cover? How large is the project? Seeing as there are six people on the team, I would assume that the project is most likely on the smaller to medium size and not very complex or special. In this case I would go with a ready-to-go cloud service. The setup would be simpler and in this way the team would have less risk of missing the release deadline. More likely to be cheaper as well. On the other hand, if the project is large and/or complex with special requirements, then there might be no other option than to self-host the environment.