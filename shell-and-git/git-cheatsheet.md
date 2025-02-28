# Creating a Remote Repository on GitHub

## 1. Log in to GitHub

- Go to [GitHub](https://github.com) and log in to your account.
- Click on **Repositories**

## 2. Create a New Repository

- Click on the **New** icon in the top-right corner and select **New repository**.
- Enter a **repository name**.
- Choose **Public** (visible to everyone) or **Private** (restricted access).
- Optionally, add:
  - A **README** file (recommended if starting fresh).
  - A **.gitignore** file to exclude unnecessary files.
  - A **license** if needed.
- Click **Create repository**.

## 3. Copy the Repository URL

- After creation, GitHub provides a **HTTPS** and **SSH** URL.
- Copy the URL based on your preference:
  - **HTTPS**: `https://github.com/yourusername/your-repo.git`
  - **SSH**: `git@github.com:yourusername/your-repo.git`

## 4. Next Steps

- If you have an existing project, initialize Git and link it:
  ```sh
  git init
  git remote add origin <REPOSITORY_URL>
  ```

## 5. Git branches and PR

### 5.1 Creating a New Branch

Create a dedicated branch for your work (feature or bug fix):

```sh
git switch -c feature/your-feature-name
```

### 5.2 Making Changes and Committing

Create a new file or edit your files and then stage and commit your changes:

```sh
git add .
git commit -m "Add: brief description of changes"
```

### 5.3 Pushing Your Branch to GitHub

Push your new branch to the remote repository:

```sh
git push origin feature/your-feature-name
```

### 5.4 Creating a Pull Request (PR)

1. Navigate to GitHub: Open your repository in a web browser.
2. Open PR: Click the "Compare & pull request" button next to your newly pushed branch.
3. Fill Details: Provide a clear title and description, and link any related issues.
4. Submit: Click "Create pull request" to submit. Explanation: These steps allow your team to review the proposed changes.

### 5.5 Addressing Feedback and Merging

- Respond to Feedback: Make any changes requested by reviewers locally, then commit and push the updates.
- Merge the PR:

  - On GitHub: Click the "Merge pull request" button once the PR is approved.
  - Via Command Line :

    ```sh
    git checkout main
    git pull origin main
    git merge feature/your-feature-name
    git push origin main
    ```
