# OC301-GitHubCheckIns
Repository for students to upload individual GitHub check-ins

# Instructions
Check-ins should be `pushed` to GitHub on every lecture day. This can be done remotely, as long as you have access to the Jupyter Server (remember that you need [OSU's VPN](https://uit.oregonstate.edu/vpn) to access the server remotely). Each GitHub check-in is worth 1\% for a total of 15\%. OC 301 has a total of 20 lectures, so you can miss up to 5 GitHub check-ins without affecting your grade.

## 1. Create a GitHub account and join our classroom (once; HW0)
After **Lecture 0**, you should have created a [GitHub](https://github.com/) account and accepted an invitation to the `OceanographicDataAnalysis` organization.

## 2. Set up ssh keys (once; HW1)
In **Lecture 1**, you will set up ssh keys on our Jupyter Server to be ready for the GitHub check-ins. Tailored instructions will be provided in HW1 and are also [available online](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent) (select 'Linux' for the server or Windows/Mac for your own computer).

## 3. Clone your own private version of this repository (once; HW1)
In **Lecture 1**, you will also `clone` your own version of this repository from GitHub to your home directory on the server. You can then attempt your first GitHub check-in.

## 4. GitHub check-in (every class day)
At the start of every new lecture (or at home on the day of the lecture if you prefer), follow the following instructions:

a) Log into the Jupyter Server

b) Open Terminal

c) Navigate to your `OC301-GitHubCheckIns-username` directory (replace `username` by your GitHub username):

    cd ~/OC301-GitHubCheckIns-username

d) `Pull` the latest version of the directory from GitHub:

    git pull

Typically, you should see the following message appear, unless you forgot to `push` your last check-in:

    Already up to date.

e) Create a new check-in file with today's date, using the command we saw in ***Lecture 0*** (the file can remain empty):

    touch HelloWorld_$(date +"%d%B%Y").txt

f) Confirm that the new file is in your directory by using `ls`:

    ls

g) `Add` all of the changed files to GitHub's staging area:

    git add .

h) `Commit` the changes by adding a note after the option `-m`:

    git commit -m 'include your note here'

i) `Push` the changes to GitHub (you might have to enter your passphrase):

    git push

<h3 align="center"><u>To receive credit for a check-in, the file must appear online on GitHub on the right lecture day.</u> </h2>

j) You can confirm that your repository is up to date with the online version on GitHub:

    git status

You should get a message that says:

    On branch main
    Your branch is up to date with 'origin/main'.

    nothing to commit, working tree clean

k) You can also go on GitHub online and confirm that there is a new file with a timestamp for just now.

If you made a mistake and changed an old file, don't worry: GitHub keeps all versions so I will be able to see when the first check-in came.

## All done! It will become easier every time.
