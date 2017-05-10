# Editing Locally

In this step we will try to start editing your Git repository from your local machine.

## Installing an editor

It is not often that I recommend a MS product but the Visual Studio Code is really good and fast enough and does well the job.

Install Microsoft Visual Studio Code in your computer.

After instalation, open a MINGW terminal and run `code .` just to check that it works well and opens the editor.

## Configuring your Git

You will need to create and add your SSH keys in Github in order to get your repository locally.

Open the terminal and follow the steps at [https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/] in order to set your enviroment up.

Now, at the terminal, create a `projects` folder:

```
mkdir projects
cd projects
```

And try to clone your repository. For doing that, go to your repo in the browser. Click at the green `Clone or download` and copy the link.

Go to the terminal and clone your repo:
```
git clone <YOUR LINK HERE>
```

If you want to clone this guide do:
```
git clone git@github.com:eargollo/training_steps.git
```

## Editing your repo

Open Visual Studio Code with your repo.

```
code Projects/<YOUR REPO PATH>
```

Mind that if you click TAB twice while writing a PATH at the terminal, the terminal will help you with the possible options. If there is only one option it will complete the PATH for you.

If you can see your README.md file at the editor, you are settled.

Create a new file, for example `cool.md` and write in it:

```
# Cool page
This is cool and I did it
```

Now push your changes to github:
```
git add . 
git commit -m "Cool file"
git push
```
Go to Github.com and check that the `cool.md` file exists there.
