# personal

A personal website that publishes to a `USERNAME.github.io` repo (only public github)

## Setup

1. Create a repo named `your-username.github.io` and replace `your-username`
2. Add it as a remote to this github repo (your source files)
   ```sh
   git remote add github-io https://github.com/your-username/your-username.github.io
   ```
3. Run the following command
   ```sh
   npm run deploy
   ```

Now your website should be deployed to `your-username.github.io`

You can read a more detailed guide about all of this [here](https://hipstersmoothie.com/blog/github-pages-user/).
