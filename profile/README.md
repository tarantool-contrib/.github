## Tarantool Contrib

Unofficial, community-maintained modules for [Tarantool](https://www.tarantool.io):
Lua rocks, C modules, tooling and everything else that grew around Tarantool but
does not belong to the core project.

> [!IMPORTANT]
> Modules here are **not** developed, supported or endorsed by the Tarantool team.
> Each repository is maintained by its own maintainers on a best-effort basis.
> For Tarantool itself and its official modules, see
> [github.com/tarantool](https://github.com/tarantool).

### Why this organization exists

- **A shared home.** A useful module should outlive its author's interest,
  job change or lost password. Here, it stays reachable and can get a new
  maintainer instead of turning into one more abandoned fork.
- **Common ground.** Shared CI templates, issue templates and conventions, so
  that moving between modules costs little.
- **Honest status.** Every repository says whether it is maintained, looking for
  a maintainer, or archived.

### Using a module

Read the module's README first: supported Tarantool versions, installation and
status are documented per repository.

A dedicated rocks server for tarantool-contrib modules is being worked out.
Until it is ready, each module's README says where to install it from.

### Bringing a module here

Have a Tarantool module that deserves a shared home? Open a
[module transfer request](https://github.com/tarantool-contrib/rfcs/issues/new/choose).
Transferring a repository keeps its stars, issues, pull requests, and
redirects from the old URL, and you stay its maintainer.

### How the organization is run

Organization-wide rules are decided as RFCs in
[tarantool-contrib/rfcs](https://github.com/tarantool-contrib/rfcs):

- [governance](https://github.com/tarantool-contrib/rfcs/blob/master/text/0002-governance.md)
  — roles, joining, module statuses, changing maintainers;
- [module requirements](https://github.com/tarantool-contrib/rfcs/blob/master/text/0003-module-requirements.md)
  — what every module repository provides.

### Getting help

- Questions about a specific module: its issue tracker.
- Questions about Tarantool itself: Tarantool community chats on Telegram, [English](https://t.me/tarantool) and [Russian](https://t.me/tarantoolru).
- Security issues: see [SECURITY.md](https://github.com/tarantool-contrib/.github/blob/master/SECURITY.md) — never file them publicly.
