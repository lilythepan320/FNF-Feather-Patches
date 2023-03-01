<p align="center">
  <h1 align="center">Friday Night Funkin': Feather</h1>
  <h2 align="center">A set of patches for Friday Night Funkin' and its various Engines!</h2>
</p>

----------------------------------------------

## Compatibility

This project aims to work with the main Friday Night Funkin' Engines in such a way no patches conflict with eachother, what are these Engines you may ask?
- [the Base Game](https://github.com/Funkin-Crew/Funkin)
- [Forever Engine](https://github.com/BeastlyGabi/Forever-Engine-Archive)
- [Psych Engine](https://github.com/ShadowMario/FNF-PsychEngine)

----------------------------------------------

## What is a patch?

What exactly is a **patch**? well, GitHub has a feature that allows for users to inject code with files, when patches are applied to a repository, every file that is specified on the patch is modified, it's kinda like making a GitHub commit but containing it on a single file

----------------------------------------------

## So then, how do I use GitHub Patches?

In order to get started with Patches, you **must** have a repository on your desired project folder, if you don't, you can easily open up a Command Prompt/Terminal and type `git init` in order to initialize an empty repository

to Apply a Patch to your repository, simply get the file of the patch you want to apply, and on your Command Prompt Window, type `git apply NAME-OF-THE-FILE.patch`

this will change all files that need to be modified in the source code

----------------------------------------------

## How do I make my own Patches?

Like stated before, GitHub Patches are like commits, you can freely make modifications to files and commit them, but instead of directly `push`ing that commit, instead, you will generate the patch file with the commit

To do that, modify the files you need, and commit them, then instead of pushing the commit, open your command prompt and type the following

`git format-patch -1`

**"Oh but I made several commits to my repository, how do I make a patch file with multiple commits?"**

instead of `-1`, specify the number of commits you've made

say that you've altered the game's Title Screen, the Main Menu, and the Options Menu, all in three commits, in this scenario, when opening the command line, we type the following

`git format-patch -3`
