# Sparse Checkout

Retrieves only the content of specific diretories in the repository.

```bash
$ mkdir examples

# make a directory we want to copy folders to
$ cd examples

# initialise the empty local repo
$ git init

# add the remote origin
$ git remote add origin -f https://github.com/xyz/abc.git

# enable sparse-checkout, configure target directories, recursivity and depth
$ git config core.sparsecheckout true
$ echo 'examples/*' >> .git/info/sparse-checkout
$ git pull --depth=2 origin master
```

See [lakehanne@github](https://lakehanne.github.io/git-sparse-checkout).