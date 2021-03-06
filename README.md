# Bobsie-Crypter

## What is this

An html file containg all the html, css and javascript to be a little username / password / credentials (and other information) storage system that is AES encrypted.

## Why?

You know how you have all kind of credentials or other login information digital and analog spread all over different places? Me too, so I created this here.

### Why html?

Compatibility of course. Everybody has a browser and you do not need any additional plugin or software and it is compatible with many different systems (not mobile optimized at the moment though).
It is just a file and the systems already have the tools, no additional stuff needed but a browsers and maybe a texteditor for nerd stuff.

## How secure is this?

More secure than the unencrypted plaintext textfiles you have lying around on your computer, but less secure than specific complex well reasoned tools programmed specifically for that purpose.
This is still vulnerable to attack vectors like keyloggers or big bruteforce attempts.
It is meant to be for private use instead of your plaintext files and maybe a little more, but do not use it of course when you have sensitive company information on computers or servers you do not trust.
If you are just a "normal person" and take at least a little care on what you do with your computers and clouds, this should be fine.

## Features

### General
* **All in one file**.
* **No extra software needed (just a browser)**.
* Table with 6 cells for one username:password entrie and descriptions or whatever you want.
* Direct **AES de- and encryption**.
* New entries can be **inserted directly** within the file itself.
* **Filter function** to just show what contains a string.
* **Edit** and **delete** existing entries.

### Details
* Dark Theme
* Filter function instantly filters on char input.
* Editing entries are saved when pressing enter.
* Auto-selects input fields depending on what you do and did. For easy navigation.
* Includes the AES library from https://github.com/ricmoo/aes-js and the SHA-256 library from https://github.com/emn178/js-sha256 implicitly and not through the include of other files.
* Use 'f' to focus the filter input, 'p' to focus password and '1' to focus the first input field to add a new entry.
* show the encrypted data in hex in the file when not decrypted.
* Copy cell-content on clicking them.

## How to use

### TL;DR
1.  ### download Bobsie-Crypter.html somewhere on your computer.
1.  ### add, change, edit as you please.
1.  ### type in password, encrypt.
1.  ### save the file (overwrite old one).

### Steps

1. Use the **password** field in the top left corner, to either encrypt or decrypt the table with your passwords. You can just hit enter when you are in the textfield, it will automatically toggle.
1. Delete or edit entries with the two buttons "delete" and "edit" in the last column.
1. Add new entries by filling the input fields "category 1", "category 2", etc. and press on add.
1. ### With your Entries in the table, just type in a password in the password field, press encrypt or hit enter and save the file (ctrl+s)! Overwrite the old file!
1. When you reopen the file, you see the encrypted content. type your password in the password field and hit enter or press decrypt, to see your list again.

### Tips & Hints
* If you messed something up, just hit **F5** to "reset" the file to the last state.
* You can easily navigate with **TAB**.
* In the password field, **ENTER** will toggle the de-/encryption depending on the current state.
* Use 'f' to select filter, 'p' to select password field and '1' for the first input field to add a new entry. (works only when you are not in an input field already)
* When you save the file in chrome, in the file dialog make sure to select the option "complete website" and not the other one (just html).

# Danger
* You can save the file also unencrypted, but do it with care.
* Don't visit bad websites with sensitive information in your clipboard! (copied).
* Don't forget your master password! The file cannot be restored in any other way. (but brute-forcing of course).
* **It is not yet deeply reviewed in a cryptographic way, but it does its job**.

## ToDo, Bugs & Technical Stuff
* Everything works so far and it's stable. I use it.
* I did **NOT** look at the very deep cryptographic situation and considered salt, other chaining algorithms, better ways to get the right key length from the password and so on, but I will probably in the future. For now, this is just a better solution for your textfiles and messy sticky notes everywhere, with a good enough encryption for non-NSA people.
* There are some little features that may be helpfull here and there, and maybe some cleaing of the code, but there are no special plans right now, I will work on them at some point when I am in the mood.
* The code still contains some unnecessary code fragments that can be stripped.
* I stuffed this together in one day, so sorry for the bad code layout and stuff, but I just wanted it to work properly first before it looks good.
* ToDo: Adding textarea or something to easyily paste old encrypted data to new version of the file.

## License

This Software (file) is published under the [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.html).
