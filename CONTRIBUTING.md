# Contributing to tarantool-contrib

Thanks for helping. This file covers every repository in the organization; a
repository may have its own `CONTRIBUTING.md` with additional, module-specific
rules, and that one wins.

## Reporting a bug

1. Check that the bug is in the module and not in Tarantool itself. If you can
   reproduce it without the module, report it to
   [tarantool/tarantool](https://github.com/tarantool/tarantool/issues).
2. Search the module's existing issues.
3. Open an issue with:
   - the module version (`tt rocks list <module>` or the commit);
   - the Tarantool version (`tarantool --version`) and OS;
   - a minimal reproducer — ideally a Lua script that runs with plain
     `tarantool script.lua`;
   - what you expected and what happened instead.

Security issues are the exception: follow [SECURITY.md](SECURITY.md) and do not
open a public issue.

## Sending a pull request

- For anything bigger than a small fix, open an issue first and agree on the
  approach with the maintainers. It saves both sides a rewritten PR.
- One logical change per commit, and a commit message that explains *why*.
- Add or update tests. Modules are tested with
  [luatest](https://github.com/tarantool/luatest); a fix comes with a test that
  fails without it.
- Keep the linter green: `luacheck .` must pass.
- Update the module's `CHANGELOG.md`, if it has one, under `Unreleased`.
- Do not bump the version in the rockspec; maintainers do that on release.

Running checks locally usually looks like this:

```sh
tt rocks make                      # install the module and its dependencies into .rocks
tt rocks install luatest
tt rocks install luacheck
.rocks/bin/luacheck .
.rocks/bin/luatest -v
```

## Review

Maintainers review on a best-effort basis, often in their spare time. If a pull
request has had no response for two weeks, a polite ping in the pull request is
welcome.

## License

By contributing, you agree that your contribution is licensed under the license
of the repository you contribute to.

## Conduct

Be reasonable. The organization owners moderate every repository and may hide
comments, lock threads, or block users who are not.
