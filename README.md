# Nostrya

Nostrya is an attempt to create distributed censorship resistant
version of github using nostr

It is developed on the grounds of:

- minimalism
- reuse of existing code and projects as much as possible
- censorship resistance

## Fundamentals

Git by its design is already very decentralized and censorship
resistant.  Yet, it lacks built-in communication layer.  Github
stepped in to solve the problem, but being a centralized organization,
it started censoring projects and people.

Git data model allows to store various types of data, including pull
requests, issues, and discussions.

To make it all work together, there should be

- presentation layer: say web interface for issues and PR's
- data availability layer that would guarantee that there's a copy of
  repository somewhere
- authentication and communication layer to identify users and message
  them
- bridges to connect to existing platforms (github, gitlab, gitea,
  etc)

Example of UI

![List of
bugs](https://user-images.githubusercontent.com/2120/223275701-8ff65ead-7624-4563-bdee-817198681d3c.png)

Loose list of functions:

- login with nostr
- create project
- delete project
- create issue
- comment on issue
- close issue
- create PR
- comment on PR
- merge PR
- close PR
