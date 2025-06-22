# ALXprodev-advanced_git

## Overview

This project is part of the **ALX Software Engineering** program and focuses on advanced Git concepts, with a strong emphasis on the **Git-Flow branching model**. The objective is to simulate real-world collaboration and gain practical experience with structured version control workflows.

## Objectives

- Initialize a Git repository and configure Git-Flow.
- Understand and implement the Git-Flow branching model.
- Manage `feature`, `release`, and `hotfix` branches effectively.
- Collaborate using standardized branching and merging strategies.

## Git-Flow Branch Types

- **main**: Contains stable, production-ready code.
- **develop**: Serves as the integration branch for ongoing development.
- **feature/**: Created from `develop` to build new features.
- **release/**: Created from `develop` to prepare a new production release.
- **hotfix/**: Created from `main` to apply urgent fixes, then merged into both `main` and `develop`.

## Project Setup

1. Install Git-Flow (if not already installed).
2. Create and clone an empty repository named `ALXprodev-advanced_git`.
3. Create a `develop` branch and push it to the remote repository.
4. Initialize Git-Flow with default settings:
   ```bash
   git flow init -d
git flow init                      # Initialize Git-Flow with default branch settings
git flow feature start <name>     # Start a new feature branch from develop
git flow feature finish <name>    # Finish the feature and merge it into develop
git flow release start <version>  # Start a release branch from develop
git flow release finish <version> # Merge release into main and develop
git flow hotfix start <version>   # Start a hotfix branch from main
git flow hotfix finish <version>  # Merge hotfix into main and develop
