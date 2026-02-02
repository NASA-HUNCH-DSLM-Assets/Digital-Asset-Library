NASA HUNCH Digital Asset Library
Security, Permissions & Folder Control Documentation

This document outlines the security rules, folder protections, team permissions, CODEOWNERS settings, and branch protection rules implemented for the NASA HUNCH Digital Asset Library.
These controls ensure a consistent, safe, and competition-compliant workflow for all participants.

1. Repository Teams and Access Levels
Artist Team

Members: You and your assigned teammates
Purpose: Creation and maintenance of required NASA models and creative models

Permissions:

Write access to:

/03_SCHOOL_SUBMISSIONS/ARTIST_TEAM/

/02_REQUIRED_MODELS/

Can create and edit folders, models, and documentation within these directories

Must submit pull requests for changes to the Shared Library

Cannot push directly to the main branch (branch protection rules apply)

Schools Team

Members: Students from participating schools
Purpose: Allow schools to contribute safely without risking damage to shared assets

Permissions:

Read-only access to the entire repository

Can fork the repository

Can submit pull requests

Cannot push directly

Cannot delete or overwrite protected folders

Cannot modify required models or shared assets

NASA Review Team

Members: NASA mentors and appointed reviewers
Purpose: Review and validate assets submitted for inclusion in the Shared Library

Permissions:

Write and approval access to:

/04_SHARED_LIBRARY/

Required approvers for pull requests affecting the Shared Library

Final authority over validated assets

Administrator / Repository Owner (You)

Permissions:

Full administrative control

Overrides CODEOWNERS where necessary

May approve any pull request

May bypass branch rules if required

Manages teams, roles, and repository security

2. CODEOWNERS Rules

Location:
.github/CODEOWNERS

These rules define ownership of specific folders and enforce required approvals.

# ============================
#  NASA HUNCH DIGITAL ASSET LIBRARY - CODEOWNERS
# ============================


# Artist Team owns all of their work
/03_SCHOOL_SUBMISSIONS/ARTIST_TEAM/*  @Artist-Team


# Artist Team owns all Required NASA Models
/02_REQUIRED_MODELS/*  @Artist-Team


# NASA Review Team controls the Shared Library
/04_SHARED_LIBRARY/*  @NASA-Review-Team


# Schools do not receive write access; they use pull requests only
# (Default GitHub permissions enforce this)


# Repository owner automatically overrides all rules
