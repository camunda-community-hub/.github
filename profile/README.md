# The Camunda Community Hub

The Camunda Community Hub is Camunda's GitHub Organization for community contributed extensions. Those extensions are independently maintained by members of the Camunda open source community (with some maintainers happen to be Camunda employees too).

With the Camunda Community Hub we want to empower our open source community to contribute, and encourage new contributors to get started contributing to the Camunda open source ecosystem.

## Existing community extensions

You can find a list of existing community extensions by [browsing the repostories](https://github.com/orgs/camunda-community-hub/repositories) in this GitHub organization.

## FAQ and further information

We’ve put together some commonly asked questions and answers on https://github.com/camunda-community-hub/community. If you have further questions, you can also ask via our [forum](https://forum.camunda.io/) or reach out to the [Camunda DevRel team](https://github.com/orgs/camunda-community-hub/teams/devrel) via email: community@camunda.com.

## How to get my community extension to the Camunda Community Hub?

- [Open an issue](https://github.com/Camunda-Community-Hub/community/issues/new/) in the [community repository](https://github.com/Camunda-Community-Hub/community/) and ask to be invited to join the Camunda Community Hub (if you are not already a collaborator).

- Sign our [CLA](https://cla-assistant.io/camunda-community-hub/community) and agree to our [Code of Conduct](https://camunda.com/events/code-conduct/). 

- Now either:

  - **Start a new community extension** by [opening an issue](https://github.com/Camunda-Community-Hub/community/issues/new/choose) using the `New Community Extension Proposal` template.
  - **Transfer your existing repository** into the Camunda Community Hub (do not fork it into the Hub). 

- Edit your extension's readme file and especially make use of [our lifecycle badges](https://github.com/Camunda-Community-Hub/community/blob/main/extension-lifecycle.md).


## How to prepare a Java project for the Camunda Community Hub?

If you develop a Java project, you can leverage the existing infrastructure for builds and releases to Maven Central.

- Use a Maven Group Id based on: `org.camunda.community`
- Add release parent pom ([as described here](https://github.com/camunda-community-hub/community-action-maven-release)):

```xml
<parent>
    <groupId>org.camunda.community</groupId>
    <artifactId>community-hub-release-parent</artifactId>
    <version>1.2.2</version>
</parent>
```

- Add Github Action [as decribed here](https://github.com/camunda-community-hub/community-action-maven-release#add-github-workflow). Check that the build is working when you push code to your repo. 

- When you are ready to release, follow [performing a release](https://github.com/camunda-community-hub/community/blob/main/RELEASE.MD#performing-a-release).


