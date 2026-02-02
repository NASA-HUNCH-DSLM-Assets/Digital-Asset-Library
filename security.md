# NASA HUNCH Digital Asset Library  
## Security, Permissions & Folder Control Documentation

This document outlines all required security rules, folder protections, team permissions, CODEOWNERS settings, and branch protection rules for the NASA HUNCH Digital Asset Library.  
It ensures a safe, standardized, competition-compliant workflow for all participants.

---

# 1. Repository Teams & Access Levels

## Artist Team
Members: You + your teammates  
Purpose: Create required NASA assets + creative models  
Permissions:
- Write access to:
  - `/03_SCHOOL_SUBMISSIONS/ARTIST_TEAM/`
  - `/02_REQUIRED_MODELS/`
- Can create/edit models, folders, templates
- Must submit PRs for Shared Library
- Cannot push directly to `main` (must use PRs)

---

## Schools Team
Members: Students from other schools  
Purpose: Allow them to contribute safely  
Permissions:
- **Read Only** access to entire repo  
- **Can Fork**
- **Can Submit Pull Requests**
- **Cannot Push**
- **Cannot Delete**
- **Cannot overwrite protected areas**

This prevents accidental corruption of models from other teams.

---

## NASA Review Team
Members: NASA mentors & official reviewers  
Purpose: Validate final assets  
Permissions:
- Write + approval access to:
  - `/04_SHARED_LIBRARY/`
- Required approvers for any PR targeting Shared Library
- Final authority for validated assets

---

## Admin / Owner (You)
Permissions:
- Full repository control  
- Automatically overrides CODEOWNERS  
- Can approve any PR  
- Can bypass protections if needed  
- Manages teams & permissions  

---

# 2. CODEOWNERS Rules

Location:  
`.github/CODEOWNERS`

These rules lock folders and assign responsibility.

```txt
# ============================
#  NASA HUNCH DIGITAL ASSET LIBRARY - CODEOWNERS
# ============================

# Artist Team owns ALL of their work
/03_SCHOOL_SUBMISSIONS/ARTIST_TEAM/*  @Artist-Team

# Artist Team also owns all Required NASA Models
/02_REQUIRED_MODELS/*  @Artist-Team

# NASA Review Team controls the Shared Library
/04_SHARED_LIBRARY/*  @NASA-Review-Team

# Schools do NOT get write access; PR-only
# (GitHub default permissions enforce this)

# Repository owner automatically overrides everything
