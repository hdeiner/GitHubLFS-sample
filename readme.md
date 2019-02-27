This project demonstrates use of GitHub with Git LFS support.

Install Git LFS under ubuntu:

```bash
$ curl -s https://packagecloud.io/install/repositories/github/git-lfs/script.deb.sh | sudo bash
$ sudo apt-get install git-lfs
$ git lfs install
```

Use Git LFS

```bash
$ git lfs track "*.mp4"
(Where *.mp4 is the pattern of filenames that you wish to track.)

$ git add .gitattributes
$ git add 2019.01.31 Chantilly Hackathon 2019! Recap.mp4
$ git add readme.md
$ git commit -m "Tracking mp4 files with Git LFS"
```

Now, when you push, things will be fine again.

For CentOS7, these are the steps to get git LFS installed:
```bash
$ sudo yum install epel-release
$ sudo yum install git
$ curl -s https://setup.ius.io/ | sudo bash
$ sudo yum install git-lfs
$ git lfs install
```