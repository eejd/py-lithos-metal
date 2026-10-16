# Local branch: what it carries relative to upstream

`local` = upstream `main` + the `topic/*` branches below. Rules: eejd/macports-ports-local
`docs/development-model.md`, "Forks, upstreams and port tiers". No `-local` port or tag exists
yet: the MacPorts port `py-lithos-metal-devel` builds upstream `main` and carries this as a
packaging patch (`patch-system-cmake.diff`).

| Change | Branch | Origin | Upstream status |
|---|---|---|---|
| Packaging and test fixes found building a MacPorts port: setup.py uses `$CMAKE` or the cmake on PATH before the cmake wheel; `test_repo_profiles_load` no longer needs the source checkout's README; the HF rotary-embedding golden tolerates transformers 5.19 | `topic/packaging-fixes` | own work (eejd/py-lithos-metal#1; squash commit 73d5e42, previously merged into this fork's `main`) | Not submitted. |
