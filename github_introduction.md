## An elementary introduction to GitHub

GitHub is the world's largest community of developers. You can upload your VE280 code to GitHub for backup and version control, collaborate with your teammates in VE280 labs and some later group projects, or even make contributions to the open-source projects of Google, Facebook, etc.

### 1. Create an account

- **Visit the homepage of GitHub:** 
<https://github.com>.

- **Pick your username.** Taking a student named "Shengyi Qian" as an example, here are several preferred naming conventions.
  - `shengyiqian`: Use the Pinyin of your full name.
  
  - `syqian` or `sqian`: If your full name is too long, say 10+ characters, you can use the acronym of your first name.
  
  - `shengyiq`: Using the acronym of your last name is also acceptable.
  
- **Enter your email and password.** Then click "Sign up for GitHub". You can change your username, email or password anytime after registration.

  ![1](images/d20542d73eb5e79f0d18e46fcb1ca9205613d56c257a41b84f2757378c5cb5d2.png)
  
- **Set up your account.** Finish the verification in Step 1. For Step 2, please select the **Free** subsciption. You can get access to the **Pro** tools later with the [GitHub Student Developer Pack](https://education.github.com/pack) (not necessary for VE280). Step 3 can be skipped.

  ![2](images/6b27e2cb53ea97567f3ec02074271e29ef6ce1637407d2bf5c8927a0ab2fe4a2.png)
  
- **Verify your email.** Open the link in the verification email sent to your registered email address. This will redirect you to the GitHub homepage. Your account has now been created!

  ![3](images/5924d5b363c9f41d1defdf915679fd8375e41b1d6ed0017ae5b161d4d3cb547c.png)

- **Visit your profile.** Click "Your profile" under your avatar at the top-right corner. Your repositories and contributions are displayed here. You can also edit the profile to add more information about yourself.

  ![4](images/2d4cab5a4ad07d68b27d90f60c15f1a4c48db8415cd2415367491542d4c74752.png)

  ![5](images/0342984ccec1794acc1dfd702642918de003df96ec752d289d36cf3538f22721.png)
  
### 2. Install Git on your local machine

- **Install Git with default packages.** Following is the Git installation command on Ubuntu. You can also install Git on Windows/Mac.

  ```
  sudo apt install git
  ```
  
- **Set up Git.** Once you have Git installed, you should configure it with your name and email address.

  ```
  git config --global user.name "Shengyi Qian"  # Replace with your name
  git config --global user.email "syqian@sjtu.edu.cn"  # Replace with your email
  ```
  
  
### 3. Use a private repository

- **Create a private repository.** Click "New" on the GitHub homepage, or simply go to <https://github.com/new>. This is the repository creation page. We usually create a repository for each project. Enter a repository name, for example, `ve280-p1-integers`. Our recommended naming convention is `lower-case-with-hyphens`. You must choose "Private" below, otherwise your code can be seen by anyone. Then check "Initialize this repository with a README" and select "C++" under "Add .gitignore". If you are interested, you could learn more about [README](https://help.github.com/en/articles/about-readmes) and [.gitignore](https://help.github.com/en/articles/ignoring-files). Click "Create repositary" at last.

  ![6](images/3e5bbee0e21c5985a23f184ab4e89d6cf1406743921092360277b86ad26be577.png)
  
- **Visit the repository page.** The URL of a GitHub repository is `https://github.com/<username>/<repository-name>`, e.g. <https://github.com/syqian/ve280-p1-integers>. There are also repository links on the GitHub homepage or your profile page.

  ![7](images/3f2b61ebd68a4352d28d3df35b7aac7f7245f426befef78240c7912893060202.png)
  
- **Clone the repository to your local machine.** Click the "Clone or download" button on your repository page and copy the URL. Then go to your Ubuntu terminal, change to some directory you'd like to store your code in, and paste the link into the `git clone` command. This will create a folder with your repository name, where you can put all the code of this project, e.g. `p1.cpp`.

  ```
  cd ~
  git clone https://github.com/syqian/ve280-p1-integers.git  # Replace with your URL
  cd ve280-p1-integers
  touch p1.cpp
  ```
  
- **Make a commit to GitHub.** 

  After you've written some code in `p1.cpp`, you need to add these changes.

  ```
  git add p1.cpp
  ```
  
  Write a message for this commit, which will be shown in your commit history.
  
  ```
  git commit -m "Finish part 1 Triangle number"
  ```
  
  Push the commit to your remote GitHub repository.
  
  ```
  git push -u origin master
  ```
  
  Now visit your repository page again and you'll find your latest update there.
  
- **Add a collaborator to your repository.**

  If you are working on a group project, you can go to the repository page and add a collaborator under "Settings" -> "Collaborators". This will send an invitation email to your teammate.
  
  ![8](images/9b7e8cc381f87efb45f5fc3a59e0a1e3c4a22c08db343e1216287a5d945e1ff7.png)
  
  After clicking "Accept invitation", your teammate will be able to access all your code and make commits to your repository too.
  
  ![9](images/8e699943b81de0ba3a74e94c1eec27d84f2ea8968edae2b45060f04eabbde9e3.png)
  

### 4. Contribute to a public repository

- **Fork a repository.** You can contribute to a public repository even if you are not one of its collaborators. Just go to the repository page, e.g. <https://github.com/ve280/ve280> (VE280 course repository), and click "Fork" at the top-right corner. The forked repository will be at `<https://github.com/<username>/ve280>`, e.g. <https://github.com/syqian/ve280>.

  ![10](images/8b343ad40192cb08ecc1a5076e9da9a9e54d07dda3ab7babbb43d6c396e886e2.png)

  ![11](images/ee3f542295777a1735f487045440fa18d917627928afe752aaa8726e0612d90c.png)

  ![12](images/a48d0cc25c9a8f2ebfc8095abce0aeb8436756bcdd9081a21ca59fbf1f7acafa.png)
  
- **Update some file.** The most common way to commit to a forked repository is exactly the same as how you commit to your own private repositories. You can `git clone` the forked repository to your local machine, make some changes, and use the `git add`, `git commit`, `git push` commands as shown in Section 3 of this tutorial. However, an alternative way is to edit some file directly on the forked repository page. Simply click a file, e.g. `README.md` on <https://github.com/syqian/ve280>, then click "Edit this file".

  ![13](images/6918f41050921fa910f0c94969273b542690b4c134c8bcc706e5385b716f489e.png)
  
  Then you can update the file content using the text editor and click "Commit changes" at the bottom of this page.
  
  ![14](images/f507fa83742d16a34786c6541e22bdf757075266237870f669a44525059447f6.png)
  
- **Create a pull request.** Visit the forked repository again, e.g. <https://github.com/syqian/ve280>. Now you should see "This branch is 1 commit ahead of ve280:master". Click the "Compare" button, then click "Create pull request" and confirm.

  ![15](images/367686b3ad061b9518fc2f08c0b5be938f9af778818350245641a21e88419419.png)

  ![16](images/c82b93beeafb55b47f3bb7fd96d92922e02e15d3a1f2791f4c5a81eb1a3d85b9.png)

  ![17](images/6204cb29b75b1e9f0f89ab60aba662da3c0c563a898e848b9fe914f8ad604d54.png)
  
  ![18](images/0094c0a5f766c268dc1490cf20fff72d6f30a60454a2568a65c8470fe8059c2e.png)
  
  Wait for one of the TAs to review your pull request. If he or she thinks you've made a good update, your commits will be merged into the main repository. Congratulations and you'll be listed in the VE280 [contributors](https://github.com/ve280/ve280/graphs/contributors)!
  
  ![19](images/d0d9de66e0d53073b027ea2a20c59013ffdd75a9b2c10267d569abf522f3d4c9.png)
  
  ![20](images/0b8b89c7cd4feb8e17645110e70937d0a9bea7bce66dfa3101e17682262203f1.png)


  
- **Star a repository.** If you like a repository, you can go to the repository page, e.g. <https://github.com/ve280/ve280>, and click "Star" at the top-right corner.
