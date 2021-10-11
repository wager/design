<p align="center">
  A GitHub mirror of Figma components.
</p>

<p align="center">
  <a href="https://github.com/wager/design/actions/workflows/mirror.yaml">
    <img
      src="https://github.com/wager/design/actions/workflows/mirror.yaml/badge.svg"
      alt="Mirror"
    />
  </a>
</p>

```bash
design/
├── .github/  # Mirror workflows.
└── branding  # Branding assets.
```

Mirror is automatically triggered every 15 minutes, but can also be [manually] triggered.

```bash
gh workflow run mirror.yaml
```

Assets can be mirrored in other repositories by adding this repository as a submodule.

```bash
git submodule add https://github.com/wager/design
```

Submodules can be kept up-to-date using [Renovate].

```json
{
  "git-submodules": {
    "enabled": true
  }
}
```

[Renovate]:
  https://github.com/renovatebot/renovate
[manually]:
  https://github.com/wager/design/actions/workflows/mirror.yaml
