# JupiterBroadcasting.com, et al. Websites

## Repo here includes issue tracking for:
  * [JupiterBroadcasting.com](https://jupiterbroadcasting.com)
  * [LINUX Unplugged](https://linuxunplugged.com/)
  * [Self-Hosted](https://selfhosted.show/)
  * [Coder Radio](https://coder.show/)
  * [Linux Action News](https://linuxactionnews.com/)
  * [Jupiter Extras](https://extras.show/)
  * [Office Hours](https://www.officehours.hair/)

## Contributing
Firstly - thank you for being here! We appreciate you.

Please read our [Contributor Guidelines](https://github.com/JupiterBroadcasting/jupiterbroadcasting.com/blob/main/CONTRIBUTING.md) on how to contribute wisely for all to benefit.

### Discussions via Matrix

Our base of operations for group discussions: [Jupiter Web Site on Matrix](https://matrix.to/#/#jupiterweb:jupiterbroadcasting.com)

---

Built with Hugo and deployed with Github Actions

Demo: https://jupiterbroadcasting.net

### Development Environment Setup

The site is deployed to production as a container and therefore we recommend development is done using docker. A convenient command in the makefile is provided to help you get started. If you're new to docker [start here](https://docs.docker.com/get-docker/).

To build and run the site run

    make dev

This will build the site (all 28000+ pages) and takes anywhere from 30s - 5 minutes depending on your hardware. This is expected due to the size of the site.

#### Deployment

Deployment is done with Github Actions, see workflow file in `.github/workflows/main.yml`
At the moment it is only triggered when something in the `main` branch is changing, but it can also be set up to run at certain times.
This would also enable scheduled publishing, since Hugo per default only builds pages which have set `date` in frontmatter to <= `now`

### Credits

- I took parts of the functionality from the Castanet Theme: https://github.com/mattstratton/castanet
Mainly the RSS feed generation and managing of hosts / guests.

- [ironicbadger](https://github.com/ironicbadger) and [JB Show Notes](https://github.com/selfhostedshow/show-notes) project which was used as the base for the [show-scraper](https://github.com/JupiterBroadcasting/show-scraper)

## Content Migration and Scraper

We moved the scraper to it's own repository here: https://github.com/JupiterBroadcasting/show-scraper
Much love to https://github.com/kbondarev aka Kiro in Matrix <3!
