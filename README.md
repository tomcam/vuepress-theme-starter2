# vuepress-theme-starter2

Adds a style sheet to the minimal custom theme for Vuepress. 

## How to use this custom theme with Vuepress

* Download this theme from GitHub into your `node_modules` directory and unzip it. You may need administrative privileges.

The result should be something like this (MacOS defaults):

```bash
$ ls /usr/local/lib/node_modules/vuepress-theme-starter2

Home.vue	Layout.vue	README.md	LICENSE
```

* Go to your working directory and create a Vuepress project. Replace ~/demo1 with whatever
you want to name your Vuepress project directory.

```bash
# Create full directory path, including the
# necessary hidden directory .vuepress
$ mkdir -p ~/demo1/.vuepress

# Make it the working directory.
$ cd ~/demo1
```
* Create a README.md file. Here it's nothing but a home page with a single h1 header.

```bash
$ echo "# hello, world." > README.md
```

* Create the file `./vuepress/config.js`:

```bash
# Replace vim with your favorite editor 
$ vim .vuepress/config.js
```

* Create this `./vuepress/config.js`:

```
const base = process.env.GH ? '/vuepress/' : '/'
module.exports = {
    title: "Demo1",
    description: "Demo of starter2 custom Vuepress theme",
    theme: "starter2"
}
```

* Generate the site and run the server:

```
$ vuepress dev
```

And visit your site at https://localhost:8080!

For a complete explanation see [Creating a minimal custom theme](http://vuepressbook.com/custom2.html).

