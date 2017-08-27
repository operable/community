Cog Project Issue Label Scheme
==============================

All issues for Cog-related repositories share a common labeling
scheme, allowing contributors to quickly find issues that they may be
interested in, or particularly suited to address. The scheme is
inspired by similar ones used by
[Rust](https://github.com/rust-lang/rust/labels),
[Habitat](https://github.com/habitat-sh/habitat/labels), and
[Kubernetes](https://github.com/kubernetes/kubernetes/labels).

# Definitions

## Area
The "area" labels indicate which area(s) of broad functionality a particular
issue is concerned with.

* `area/adaptor`
  General chat adaptor interface
* `area/adaptor/hipchat`
  Issues specific to the HipChat adapter
* `area/adaptor/slack`
  Issues specific to the Slack adapter
* `area/api`
  The Cog REST API
* `area/build`
  Issues around CI, release tooling, packaging, etc.
* `area/cli`
  The `cogctl` command-line interface
* `area/commands`
  Chat commands
* `area/documentataion`
  General project documentation
* `area/executor`
  The main command executor loop in the Cog server
* `area/relay`
  The Relay command execution agent
* `area/rules`
  Cog's permission rule system
* `area/testing`
  Testing infrastructure, including command bundle testing

## Effort
The "effort" labels give a rough idea of the amount of work it should take to
address a particular issue. The labels should be self-explanatory; people
interested in getting involved with Cog for the first time should pay particular
attention to the `effort/easy` label.

* `effort/easy`
* `effort/medium`
* `effort/difficult`

## Flag
The "flag" labels are general process-related labels that help the Cog
maintainers manage the overall project.

* `flag/needs-discussion`
  This issue needs more discussion with community members and maintainers to
  decide on a course of action.
* `flag/waiting-for-response`
  A maintainer has requested feedback from the submitter of an issue or PR.

## Type
This group of labels indicate the general kind of issue.

* `type/bug`
  Assigned to reported problems in the code.
* `type/chore`
  Issues that "just need to be done"... improving the build process, updating
  runtime dependencies, and so on. These don't address bugs, or add new
  functionality, but are necessary to the continued health and maturation of the
  project.
* `type/feature`
  Added to requests or ideas for new functionality or behavior.

# Maintenance

To keep labels up-to-date and consistent across repositories, we use
[Repo Gopher](https://github.com/ohaiwalt/repo-gopher), itself
inspired by [Repo Man](https://github.com/thommay/repo_man).

All label definitions are contained in [config.toml](config.toml).

To run it:

``` sh
export GITHUB_AUTH_TOKEN=XXXXXXXXXXXXXXXXXX
make
```
