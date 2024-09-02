Built a small Git implementation that's capable of
initializing a repository, creating commits and cloning a public repository.
Learnt about the `.git` directory, Git objects (blobs,
commits, trees etc.), Git's transfer protocols and more.




# Testing locally

The `your_program.sh` script is expected to operate on the `.git` folder inside
the current working directory. If you're running this inside the root of this
repository, you might end up accidentally damaging your repository's `.git`
folder.

Execute `your_program.sh` in a different folder when testing
locally. For example:

```sh
mkdir -p /tmp/testing && cd /tmp/testing
/path/to/your/repo/your_program.sh init
```

To make this easier to type out, you could add a
[shell alias](https://shapeshed.com/unix-alias/):

```sh
alias mygit=/path/to/your/repo/your_program.sh

mkdir -p /tmp/testing && cd /tmp/testing
mygit init
```
