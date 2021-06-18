# jsdoc-template-hypergrid

Originally a clone of [Default JSDoc template](https://github.com/jsdoc3/jsdoc/tree/master/templates/default), since modified.

## Submodule cloning

When cloning a repo that references this submodule,
be sure to give the `--recurse-submodules` option to clone the
contents of the submodule:

```bash
git clone --recurse-submodules https://github.com/fin-hypergrid/rectangular.git
```

If you forget, you can still do it (soon) after cloning as a separate command:

```bash
git clone https://github.com/fin-hypergrid/rectangular.git
git submodule update --init --recursive
```

### New repo

To add this template to a new repo in a `jsdoc-template` folder (after `git clone` or `git init`):

```shell
git submodule add https://github.com/fin-hypergrid/jsdoc-template-hypergrid jsdoc-template
```
 
These changes will then need to be committed.
 
### Re-purpose an existing clone that already uses this submodule

Sometimes it is useful to use an existing repo as a template for a new repo.
But, like the existing repo, you want to reference the submodule (rather than copying it).

```shell
cp existing-repo new-repo
cd new-repo
rm -fdr .git
rm .gitmodules
git init
rm -drf jsdoc-template/
```
 
Then proceed as for [New repo](newrepo).
 
