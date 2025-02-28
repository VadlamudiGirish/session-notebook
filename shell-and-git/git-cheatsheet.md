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
