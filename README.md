# dev



## Getting started

## **Pre-required Software**

- **XAMPP**
  - Download and install from [https://www.apachefriends.org/](https://www.apachefriends.org/)
  - Depending on your OS, select either the Windows, Linux, or Mac installer

- **Node.js**
  - Install from [https://nodejs.org/en/download](https://nodejs.org/en/download)
  - Depending on your OS, select from Windows, Linux, Mac, or AIX

- **IntelliJ IDEA**
  - Download from [https://www.jetbrains.com/idea/download/?section=windows](https://www.jetbrains.com/idea/download/?section=windows)
  - If you have a JetBrains subscription, use the Ultimate edition; otherwise, use the FREE Community edition

- **JDK 21**
  - Install from [https://www.oracle.com/java/technologies/downloads/#java21](https://www.oracle.com/java/technologies/downloads/#java21)
  - Select the installer for your OS

- **JDK 17**
  - Install from [https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html)
  - Select the installer for your OS
  - **Note:** As of now, Calories Count requires both JDK 21 & 17 to operate. This will hopefully be fixed to only require 21 in the future.

---

## **Setting up Calories Count**

- **Open Calories Count in IntelliJ**
  - In IntelliJ, select `New -> Project`
  - Navigate to where Calories Count is saved and select the folder

- **Build Gradle**
  - In IntelliJ, navigate to: `/dev/build.gradle.kts`
  - Inside `build.gradle.kts`, click the **Link** button in the top-right corner
  - Wait patiently for IntelliJ to finish linking the Gradle file (this may take some time)

- **Set up MySQL and Apache**
  - Open the **XAMPP Control Panel**
  - Start **Apache** and **MySQL**
  - Once both have started, click the **Admin** button next to MySQL

- **Start Calories Count Backend**
  - In IntelliJ, navigate to: `/dev/src/main/kotlin/com/example/test3/Test3Application.kt`
  - Run `fun main()` using the green arrow next to it, or the larger green arrow in the top-right corner of IntelliJ

- **Set up Database**
  - In PHPMyAdmin (opened from the XAMPP Control Panel), locate the `caloriescount` DB created by the backend
  - Run the following SQL script to populate the DB:
    ```sql
    -- Yet to be provided Script --
    ```

- **Start Calories Count Frontend**
  - In IntelliJ, open the in-app terminal (Alt + F12)
  - Run one of the following commands depending on your OS:
    - Windows: `cd .\UI\`
    - Unix: `cd /UI/`
    - Alternatively: `cd ui`
  - Install NPM dependencies: `npm install`
  - Build the project: `npm run build`
  - Start the frontend: `node server.js`
  - If done properly, click the URL provided or navigate to [https://localhost:5173](https://localhost:5173) to view Calories Count


## Add your files

- [ ] [Create](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#create-a-file) or [upload](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#upload-a-file) files
- [ ] [Add files using the command line](https://docs.gitlab.com/ee/gitlab-basics/add-file.html#add-a-file-using-the-command-line) or push an existing Git repository with the following command:

```
cd existing_repo
git remote add origin https://gitlab.com/ru-softeng/sp25-370/team04/dev.git
git branch -M main
git push -uf origin main
```

## Integrate with your tools

- [ ] [Set up project integrations](https://gitlab.com/ru-softeng/sp25-370/team04/dev/-/settings/integrations)

## Collaborate with your team

- [ ] [Invite team members and collaborators](https://docs.gitlab.com/ee/user/project/members/)
- [ ] [Create a new merge request](https://docs.gitlab.com/ee/user/project/merge_requests/creating_merge_requests.html)
- [ ] [Automatically close issues from merge requests](https://docs.gitlab.com/ee/user/project/issues/managing_issues.html#closing-issues-automatically)
- [ ] [Enable merge request approvals](https://docs.gitlab.com/ee/user/project/merge_requests/approvals/)
- [ ] [Set auto-merge](https://docs.gitlab.com/ee/user/project/merge_requests/merge_when_pipeline_succeeds.html)

## Test and Deploy

Use the built-in continuous integration in GitLab.

- [ ] [Get started with GitLab CI/CD](https://docs.gitlab.com/ee/ci/quick_start/)
- [ ] [Analyze your code for known vulnerabilities with Static Application Security Testing (SAST)](https://docs.gitlab.com/ee/user/application_security/sast/)
- [ ] [Deploy to Kubernetes, Amazon EC2, or Amazon ECS using Auto Deploy](https://docs.gitlab.com/ee/topics/autodevops/requirements.html)
- [ ] [Use pull-based deployments for improved Kubernetes management](https://docs.gitlab.com/ee/user/clusters/agent/)
- [ ] [Set up protected environments](https://docs.gitlab.com/ee/ci/environments/protected_environments.html)
