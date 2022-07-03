# language_flashcards - tsv files to learn languages

I use this .tsv files with
[vocage](https://github.com/proycon/vocage), a vocabulary learning
tool made with rust. Remember to use tabs to separate columns. if
you're using an editor that writes spaces instead of tabs by default,
make a rule for tsv files to override that behavior:

```bash
# Example for neovim
mkdir -p ~/.config/nvim/after/ftplugin
cd ~/.config/nvim/after/ftplugin
echo "setlocal ts=2\nsetlocal sw=2\nsetlocal noexpandtab" > tsv.vim
```

# Install/Setup

This is my personal setup, so feel free to do whatever you want instead.

```bash
# Do this the first time only
git clone https://github.com/mFragaBA/language_flashcards ~/.vocage/language_flashcards

# This is optional, but i usually create a second file on 
# which i run vocage on and whenever I update the definition 
# file, I just copy the new lines into my current file
cd ~/.vocage/language_flashcards/kr
cp define_topki1.tsv topik1.tsv

# Usage example
cd ~/.vocage/language_flashcards/kr
vocage topik1.tsv
```
