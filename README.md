# tmpl - the superlight project template manager

`tmpl` is an all bash command line utility for managing personal project templates. It's main aim is to be small and easy to use while having enough functionality to kick start most projects.

All it does is copy the template from a source to a destination, reinitialize the git repository and run a `tmpl-init` script if it exists in the template.

## Setup

To install `tmpl` globally run to install it to the global context

```
sudo cp ./tmpl /usr/local/bin/
```

If you only want it to install for your user, you can install it somewhere in your home and add it to your path.

```
mkdir ~/.tmpl
cp ./tmpl ~/.tmpl/
```

Then add that to your path in your runtime config for your chosen shell, `.bashrc` or `.zshrc` example below.

```
export PATH=$PATH:$HOME/.tmpl/
```

The last step is to tell it where your project templates live, you can either also add that to your `.bashrc` or similar or you can create a `.tmplrc` in your home.

If in `.bashrc` or `.zshrc`

```
export PROJECT_TEMPLATES_DIR=<your directory>
```

if in `.tmplrc` you put

```
PROJECT_TEMPLATES_DIR=<your directory>
```

## Usage

`tmpl` only has two commands `ls` and `init`. `ls` will list templates and init will initialize that template into the directory specified.

You can get the full usage by running `tmpl` without arguments.


