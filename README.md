# ensf400-project-group22

## Git Workflow

### Branching Strategy
- `main`: Production-ready branch. No direct commits should occur in this branch.
- `dev`: Development branch. Individual features are merged here before being merged to `main`.
- `feature-*`: Feature branches. Used for bug fixes/new functionalities.

### New Branch Creation
Change branches to `dev` branch then create new branch off of it:  
   ```bash
   git checkout dev
   git pull origin dev
   git checkout -b feature-name
   git push origin feature-name
```

### Pull Requests\Code Reviews
When merging into another branch, a pull request is necessary
 before this happens. It must include a short description of what has been changed. At least one other team member must review the code for quality and consistency, and approve the request. Once a feature has been merged to `dev` and it has been tested, `dev` can be merged into `main`.