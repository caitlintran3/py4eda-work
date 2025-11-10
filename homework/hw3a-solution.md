# HW3A Solution - Git and Version Control
## Part 1: Repository Cloning
I successfully cloned the class repository from `https://github.com/olearydj/INSY6500` to
`~/insy6500/class_repo`.
### Key Commands Used
- `git clone <url>` - Create local copy of remote repository
- `git log` - View commit history
- `git remote -v` - Check remote repository connections
## Part 2: Portfolio Repository Creation
I created my personal course repository with:
- Professional README.md describing the project
- Proper .gitignore to exclude unnecessary files
- Organized directory structure for homework, projects, and notes
### Understanding Git Workflow
The three-stage workflow:
1. Working Directory: Where I edit files
2. Staging Area: Where I prepare commits with `git add`
3. Repository: Where commits are permanently stored with `git commit`
## Part 3: GitHub Publishing
Successfully published repository to GitHub:
- Used `git remote add origin` to connect local repo to GitHub
- Used `git push -u origin main` to upload commits
- Verified all files and commits are visible on GitHub
### The Remote Connection
My local repository is now connected to GitHub:
- `git remote -v` shows the remote URL
- `git push` will send my commits to GitHub
- `git pull` will get updates from GitHub (if changes are made on GitHub)
### Details
Complete this section with details from your setup:
- Repository URL: ...
- Output of `git remote -v`:
- The output of `git log --oneline`:
## Questions

### Reflections

1. **What did you learn about Git and GitHub?**  
I learned how Git tracks changes locally and how GitHub serves as a remote platform for sharing and collaboration. Setting up a repository from scratch helped me understand how commits, remotes, and branches work together. I also got more comfortable using the command line and troubleshooting authentication issues.

2. **What was the most confusing part?**  
Authentication was the hardest part. Between personal access tokens, SSH keys, and GitHub permissions, it took several tries to get everything working. I also had to be careful with file paths and staging changes correctly—Git’s error messages can be vague if something goes wrong.

3. **What would you do differently next time?**  
Next time, I’d set up SSH from the beginning to avoid token issues. I’d also double-check my folder structure before committing and make sure I’m always working in the correct directory. That would’ve saved me a lot of time.

### Graduate Questions

1. **What are the pros and cons of SSH vs HTTPS for GitHub authentication?**  
SSH is more secure and convenient once it’s set up, since it doesn’t require entering a token every time. HTTPS is easier to start with, but managing tokens can be frustrating. SSH also works better for automation and scripting.

2. **How would you automate this workflow for future assignments?**  
I’d write a shell script that sets up the folder structure, initializes the repo, adds the remote, and pushes the first commit. I’d also include a template README and .gitignore so I don’t have to recreate them each time.

3. **How does Git support reproducibility in research?**  
Git tracks every change, so it’s easy to see how a project evolved. You can roll back to earlier versions, compare results across branches, and collaborate without overwriting each other’s work. That makes it ideal for reproducible research and versioned data analysis.
