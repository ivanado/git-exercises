# Exercise 5: Create your repository


# Create your GitHub repository
1. Log-in to [GitHub](www.github.com)
1. Go to Repositories -> New
    - Name it `my-demo-repo`
    - Add a description: *git-workshop repository for experimenting with basic git operations*
    - Keep it **Public** (you can change this later)
    - Check `Add a README file`
    - Ignore the .gitignore template
    - Ignore the licensing dropdown at this point
    - Click `Create repository`

# Clone your repository
1. Go to your GitHub repository page
1. Click `Code`
    - Choose HTTPS
    - Copy the URL
1. In your terminal run:
``` bash 
git clone <copied_URL>
# i.e.: git clone https://github.com/rodik/my-demo-repo.git
```
4. In your terminal run: `cd my-demo-repo`
4. You are ready to start working!

# Create, stage, commit and push a file
Run the following commands in your terminal:
``` bash
# 1. Create a new file by running 
echo "hello triangle" > newfile.txt
# 2. Stage the file
git add newfile.txt
# 3. Commit the file
git commit -m "adding my first file"
# 4. Push the file
git push
```
> This is a simplified version of the process

### Tips and tricks:
1. [gh cli](https://cli.github.com/) - command line interface for GitHub
1. [Choosing](https://choosealicense.com/) an open source license
