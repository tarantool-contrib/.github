# tarantool-contrib/.github

Organization-wide defaults for [tarantool-contrib](https://github.com/tarantool-contrib).

GitHub uses the files in this repository for every repository in the
organization that does not have its own copy:

- `profile/README.md` — the organization's public profile page;
- `CONTRIBUTING.md`, `SECURITY.md`, `SUPPORT.md` —
  default community health files;
- `.github/ISSUE_TEMPLATE/`, `.github/PULL_REQUEST_TEMPLATE.md` — default issue
  and pull request templates;
- `workflow-templates/` — starter GitHub Actions workflows offered on the
  "Actions → New workflow" page of every repository.

A repository overrides any of these by adding a file with the same name. Note
that the override is per file: a repository with its own `ISSUE_TEMPLATE/`
directory gets none of the templates from here.

## Workflow templates

- **Tarantool module: test** — luacheck and a luatest run over a matrix of
  Tarantool versions.

It assumes the common module layout: a `<name>-scm-1.rockspec` in the
repository root, tests under `test/` runnable with luatest, and a
`.luacheckrc`.

A starter for publishing rocks will follow once the organization's rocks
server is settled; that part is still being worked out.
