# Git Branching Strategy

## 1. Branch Types

### main
- This is the production branch.
- Always reflects the latest stable release.
- Only thoroughly tested and reviewed code is merged into `main`.

### feature branches
- Used for developing new features or enhancements.
- Always branch off from `main`.
- Naming convention: `feature/<short-description>` (e.g., `feature/user-authentication`)
- Once complete, create a pull request (PR) into `main` after review and testing.

## 2. Workflow

1. **Start a new feature**  
   ```bash
   git checkout main
   git pull origin main
   git checkout -b feature/<feature-name>
