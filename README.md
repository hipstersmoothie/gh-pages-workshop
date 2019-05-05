# gh-pages workshop

This repository will show you all the different ways to utilized GitHub pages to document and show off your projects.

GitHub pages is a static website that is available to any project on GitHub. There are a few different ways to use pages:

| Type                  | Use Case                                                                                  |
| --------------------- | ----------------------------------------------------------------------------------------- |
| Master                | You have a website with no build step and the files in master constitute only the website |
| Master `docs/` folder | Your project is in master and you have a no build website in the `docs/` folder           |
| gh-pages branch       | You have some sort of build step for your website that outputs to a `dist` folder         |

In most cases a `gh-pages` branch is the way to go. It allows you to put whatever you want in it and keep you repository clean of build files

## Branches

This repo has a branch that demonstrates some different use cases for deploying things to GitHub pages.

1. `simple` - A simple no build website
2. `cra` - A create-react-app that deploys to the `gh-pages` folder
3. `storybook` - A storybook that deploys to the `gh-pages` folder
4. `personal` - A personal website that publishes to a `USERNAME.github.io` repo (only public github)

## Creating the gh-pages branch

The following are the command you should run to create a GitHub pages branch in your repo.

```sh
# Create an orphan branch
git checkout --orphan gh-pages
# Remove all previous files
rm .git/index	&& git rm -rf *
# Create the first commit so we push
git clean -fdx && git commit --allow-empty -m "empty commit"
# Push the branch to your remote
git push -u origin gh-pages
```
