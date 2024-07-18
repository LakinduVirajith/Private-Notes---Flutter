# Private Notes
A new Flutter project for managing private notes with Firebase integration.

## Table of Contents
- [Private Notes](#private-notes)
  - [Table of Contents](#table-of-contents)
  - [Getting Started](#getting-started)
  - [Project Setup](#project-setup)
    - [Creating the Flutter Project](#creating-the-flutter-project)
  - [Firebase CLI](#firebase-cli)
  - [FlutterFire Setup](#flutterfire-setup)
    - [FlutterFire Initialization](#flutterfire-initialization)
  - [Firebase Configuration](#firebase-configuration)
  - [Firebase Dependencies](#firebase-dependencies)
    - [Firebase core](#firebase-core)
    - [Firebase auth](#firebase-auth)
    - [Cloud firestore](#cloud-firestore)
    - [Firebase analytics](#firebase-analytics)
  - [Basic Git Commands](#basic-git-commands)
    - [git init](#git-init)
    - [git clone](#git-clone)
    - [git status](#git-status)
    - [git add](#git-add)
    - [git commit](#git-commit)
    - [git diff](#git-diff)
    - [git log](#git-log)
    - [git branch](#git-branch)
    - [git checkout](#git-checkout)
    - [git merge](#git-merge)
    - [git remote](#git-remote)
    - [git push](#git-push)
    - [git pull](#git-pull)
  - [Advanced Git Commands](#advanced-git-commands)
    - [git fetch](#git-fetch)
    - [git rebase](#git-rebase)
    - [git reset](#git-reset)
    - [git revert](#git-revert)
    - [git stash](#git-stash)
    - [git tag](#git-tag)
    - [git log --oneline](#git-log---oneline)
    - [git rm](#git-rm)
    - [git mv](#git-mv)
    - [git config](#git-config)
  - [Git Workflow Commands](#git-workflow-commands)
    - [git cherry-pick](#git-cherry-pick)
    - [git blame](#git-blame)
    - [git show](#git-show)
    - [git archive](#git-archive)
    - [git submodule](#git-submodule)
    - [git bisect](#git-bisect)
  - [Usage](#usage)
  - [Resources](#resources)

## Getting Started
This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.

## Project Setup
### Creating the Flutter Project

To create the Flutter project, run the following command:
```
flutter create --org se.pixolity private_notes
```
This flag specifies the organization identifier for your project.
This helps uniquely identify your app and is used as the package name for Android and the bundle identifier for iOS.

## Firebase CLI
To use Firebase CLI for various tasks, follow these steps:

1. Install Firebase CLI:
```
npm install -g firebase-tools
```
2. Log in to Firebase:
```
firebase login
```

## FlutterFire Setup
This project uses Firebase for backend services such as authentication and cloud storage. Follow the steps below to set up Firebase for your project.

### FlutterFire Initialization

FlutterFire is the set of Flutter plugins that enable Flutter apps to use Firebase services.

1. Visit the [FlutterFire Overview](https://firebase.flutter.dev/docs/overview/) for an introduction.
2. Install the FlutterFire CLI if you haven't already:
```
dart pub global activate flutterfire_cli
```
1. Run the configure command to select a Firebase project and platforms:
```
flutterfire configure
```

## Firebase Configuration
After configuring FlutterFire, set up your Firebase project in the Firebase console:

1. Go to the [Firebase Console.](https://firebase.google.com/docs/cli#install-cli-windows)
2. Configure authentication methods such as Email/Password, Google Sign-In, and Facebook Login.

## Firebase Dependencies
Add the following dependencies to your pubspec.yaml file for Firebase integration:

### Firebase core
Initializes Firebase in the Flutter project.
yaml
```
dependencies:
  firebase_core: latest_version
```
### Firebase auth
Provides Firebase authentication services.
yaml
```
dependencies:
  firebase_auth: latest_version
```
### Cloud firestore
Enables access to Firestore database.
```
dependencies:
  cloud_firestore: latest_version
```
### Firebase analytics
Tracks user events and analytics.
```
dependencies:
  firebase_analytics: latest_version
```

## Basic Git Commands
### git init
- Initializes a new Git repository in the current directory.
- Usage: `git init`

### git clone
- Clones an existing repository from a remote server to your local machine.
- Usage: `git clone <repository_url>`

### git status
- Shows the status of changes as untracked, modified, or staged.
- Usage: `git status`

### git add
- Adds files to the staging area.
- Usage: `git add <file_name>`
- To add all files: `git add .`

### git commit
- Records changes to the repository with a descriptive message.
- Usage: `git commit -m "commit message"`

### git diff
- Shows the differences between the working directory and the staging area.
- Usage: `git diff`

### git log
- Shows the commit history.
- Usage: `git log`

### git branch
- Lists all branches in the repository.
- Usage: `git branch`
- To create a new branch: `git branch <branch_name>`

### git checkout
- Switches to a different branch.
- Usage: `git checkout <branch_name>`
- To create and switch to a new branch: `git checkout -b <branch_name>`

### git merge
- Merges a branch into the current branch.
- Usage: `git merge <branch_name>`

### git remote
- Manages remote repository connections.
- Usage: `git remote`
- To add a remote: `git remote add <name> <url>`

### git push
- Pushes changes from the local repository to a remote repository.
- Usage: `git push <remote> <branch>`

### git pull
- Fetches and integrates changes from a remote repository to the local repository.
- Usage: `git pull <remote> <branch>`

## Advanced Git Commands
### git fetch
- Fetches changes from a remote repository without merging them.
- Usage: `git fetch <remote>`

### git rebase
- Reapplies commits on top of another base tip.
- Usage: `git rebase <branch>`

### git reset
- Resets the current HEAD to a specified state.
- Usage: `git reset <commit>`
- To unstage changes: `git reset <file_name>`

### git revert
- Creates a new commit that undoes changes made by a previous commit.
- Usage: `git revert <commit>`

### git stash
- Temporarily stores changes that are not ready to be committed.
- Usage: git stash
- To apply stashed changes: `git stash apply`

### git tag
- Creates a tag for a specific commit.
- Usage: `git tag <tag_name>`

### git log --oneline
- Shows the commit history in a single line format.
- Usage: `git log --oneline`

### git rm
- Removes files from the working directory and the staging area.
- Usage: `git rm <file_name>`

### git mv
- Moves or renames a file, directory, or symlink.
- Usage: `git mv <source> <destination>`

### git config
- Configures Git settings.
- Usage: `git config --global user.name "Your Name"`
- To set email: `git config --global user.email "you@example.com"`

## Git Workflow Commands
### git cherry-pick
- Applies the changes introduced by some existing commits.
- Usage: `git cherry-pick <commit_hash>`

### git blame
- Shows what revision and author last modified each line of a file.
- Usage: `git blame <file_name>`

### git show
- Displays information about a specific commit.
- Usage: `git show <commit>`

### git archive
- Creates an archive of files from a named tree.
- Usage: `git archive --format=zip HEAD > archive.zip`

### git submodule
- Manages submodules (repositories within a repository).
- Usage: `git submodule add <repository_url>`

### git bisect
- Helps to find the commit that introduced a bug by binary search.
- Usage: `git bisect start`

## Usage
Follow the setup instructions above to configure your Flutter project with Firebase. Once everything is set up, you can run the project using:

```
flutter run
```
## Resources
[Flutter Documentation](https://docs.flutter.dev/)

[Firebase Documentation](https://firebase.google.com/docs)

