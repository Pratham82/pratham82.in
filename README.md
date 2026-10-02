# pratham82.in

Parent repo for [pratham82.in](https://pratham82.in). The two apps live in their own repos and are included here as git submodules, so their PRs, CI and deploys stay separate.

| Folder | Repo | What | Deploys to |
| --- | --- | --- | --- |
| [`frontend/`](frontend) | [Pratham82/portfolio-v5](https://github.com/Pratham82/portfolio-v5) | Next.js site | Vercel |
| [`backend/`](backend) | [Pratham82/portfolio-api](https://github.com/Pratham82/portfolio-api) | Sanity Studio and schema | `sanity deploy` |

## Clone

```bash
git clone --recurse-submodules git@github.com:Pratham82/pratham82.in.git
```

Already cloned without submodules: `git submodule update --init`.

## Day to day

Work inside `frontend/` or `backend/` as normal repos: branch, commit, push and open PRs there.

This repo only records which commit of each app it points at. To move it to the latest `master` of both:

```bash
git submodule update --remote
git commit -am "chore: 🤖 bump submodules"
```
