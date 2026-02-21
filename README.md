.
├── apps
│   ├── core
│   │   └── ingress.yaml           # The shared ALB definition
│   └── data-api
│       ├── deployment.yaml
│       ├── service.yaml
│       └── ingress.yaml           # The route injection
├── core-app-definition.yaml       # Tells Argo to sync 'core'
├── data-api-app-definition.yaml   # Tells Argo to sync 'data-api'
├── gitops-repo-secret.yaml
└── root-app.yaml                  # Points to the two definitions above