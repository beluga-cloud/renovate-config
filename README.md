<!-- markdownlint-disable MD033 -->
<h1 align="center">
  <a href="https://github.com/belug-apps">
    <img src="https://github.com/belug-apps/.github/raw/main/assets/logo_400px.png" alt="Logo" width="150" height="150">
  </a>
</h1>

<h4 align="center">Belug-Apps - TrueCharts alternative for TrueNAS SCALE</h4>

<div align="center">
  <br/>

  [
    ![License](https://img.shields.io/github/license/belug-apps/belug-apps?logo=git&logoColor=white&logoWidth=20)
  ](LICENSE)
  [
    ![Pending dependencies](https://img.shields.io/github/issues-pr/belug-apps/renovate-config/type:%20dependencies?label=dependencies&logo=renovatebot&logoWidth=20&style=flat)
  ](https://github.com/belug-apps/renovate-config/pulls?q=is%3Apr+is%3Aopen+label%3A%22type%3A+dependencies%22)

</div>

---
<!-- markdownlint-enable MD033 -->

## Renovate presets

This repository contains all Renovate presets used inside the Belug-Apps organisation.

### [Why we should use presets ?](https://docs.renovatebot.com/key-concepts/presets/)

Use presets to:

- Set up the bot with good default settings
- Reduce duplication of your configuration
- Share your configuration with others
- Use somebody else's configuration and extend it with your own rules

### Managing config for many repositories

If you manage Renovate for many repositories, then you should create a global preset configuration. Then you extend the global preset in each repository. This way you have all global configuration in a single file, in a single repository.

## List of existing presets

- `github>belug-apps/renovate-config:gitmoji`: make every Renovate commits compatible with [Gitmoji](https://gitmoji.dev/).
- `github>belug-apps/renovate-config:github-actions({{schedule}})`: groups all github-actions upgrades together to reduce the number of PRs.
  - `{{schedule}}`: defines when Github actions upgrade should be scheduled. Must be one of `daily`, `earlyMondays`, `monthly`, `nonOfficeHours`, `quarterly`, `weekdays`, `weekends`, `weekly` or `yearly`
- `github>belug-apps/renovate-config:asdf({{schedule}})`: groups all ASDF upgrades together to reduce the number of PRs.
  - `{{schedule}}`: defines when Github actions upgrade should be scheduled. Must be one of `daily`, `earlyMondays`, `monthly`, `nonOfficeHours`, `quarterly`, `weekdays`, `weekends`, `weekly` or `yearly`
