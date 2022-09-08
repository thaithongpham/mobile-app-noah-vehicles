# mobile-app-noah-vehicles

# GIT Branches 
1. The main branches 
- main branch 
To be the main branch where the source code of HEAD always reflects a production-ready state.

- developer branch  
the source code of HEAD always reflects a state with the latest delivered development changes for the next release.

When the source code in the develop branch reaches a stable point and is ready to be released, all of the changes should be merged back into the master and then tagged with a release number.

2. The supporting branches 
- Feature branches: 	
May branch off from:
develop
Must merge back into:
develop
Branch naming convention:
Anything except master, develop, release-*, or hotfix-*

Feature branches (or sometimes called topic branches) are used to develop new features for the upcoming or a distant future release. 

- Release branches 
Release branches 
May branch off from:
develop
Must merge back into:
develop and master
Branch naming convention:
release-*

Release branches support the preparation of a new production release. They allow for last-minute dotting of i’s and crossing t’s. Furthermore, they allow for minor bug fixes and preparing meta-data for a release (version number, build dates, etc.). By doing all of this work on a release branch, the develop branch is cleared to receive features for the next big release.

- Hotfix branches 
May branch off from:
master
Must merge back into:
develop and master
Branch naming convention:
hotfix-*

Hotfix branches are very much like release branches in that they are also meant to prepare for a new production release, albeit unplanned. They arise from the necessity to act immediately upon an undesired state of a live production version. When a critical bug in a production version must be resolved immediately, a hotfix branch may be branched off from the corresponding tag on the master branch that marks the production version.