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
$ git commit -m "track *.mp4 files using Git LFS"

$ git add *.mp4
$ git commit -m "add mp4 file"

Now, when you push, things will be fine again.

```