# ArgoCD Render Manifests Action

Use helmfile to render application manifests for use with ArgoCD

### Inputs

| Name                        | Required | Default | Description                                                                                        |
| --------------------------- | :------: | ------- | -------------------------------------------------------------------------------------------------- |
| `app`                       |    ✅    | `n/a`   | The app to render manifests for.                                                                   |
| `cluster`                   |    🚫    | `""`    | The cluster to render manifests against.                                                           |
| `remove_disabled_manifests` |    🚫    | `false` | Remove manifests for clusters the app is disabled in.                                              |
| `namespace`                 |    🚫    | `""`    | The application destination namespace. If not set will be discovered.                              |
| `app_deploy_config_dir`     |    🚫    | `""`    | The base directory for app deployment config. If not set will be inferred using the app name.      |
| `manifest_dir`              |    🚫    | `""`    | The directory to sync rendered manfiests to relative to project root. If not set will be inferred. |
