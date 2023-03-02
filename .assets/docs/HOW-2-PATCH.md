<h1 align="center">
So then, how do I use GitHub Patches?
</h1>

In order to get started with Patches, you **must** have a repository on your desired project folder, if you don't, you can easily open up a Command Prompt/Terminal and type `git init` in order to initialize an empty repository

- If you came from the [Submissions](SUBMISSIONS.md) section, you can just ignore this

to Apply a Patch to your repository, simply get the file of the patch you want to apply, move it to your project's root folder, and on your Command Prompt Window, type `git apply NAME-OF-THE-FILE.patch`

this will change all files that need to be modified in the source code

----------------------------------------------

<h1 align="center">
How do I make my own Patches?
</h1>

Like stated before, GitHub Patches are like commits, you can freely make modifications to files and commit them, but instead of directly `push`ing that commit, instead, you will generate the patch file with the commit

To do that, modify the files you need, and commit them, then instead of pushing the commit, open your command prompt and type the following

`git format-patch -1`

<h3 align="center">
"Oh but I made several commits to my repository, how do I make a patch file with multiple commits?"
</h3>

instead of `-1`, specify the number of commits you've made

say that you've altered the game's Title Screen, the Main Menu, and the Options Menu, all in three commits, in this scenario, when opening the command line, we type the following

`git format-patch -3`

this will generate a file with the commit names, ending in `.patch`, you can then distribute this patch file accordingly.