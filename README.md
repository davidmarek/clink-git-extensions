# clink-git-extensions

This repository currently consists of two LUA extensions for [clink](https://mridgers.github.io/clink/):

* `git_alias_autocomplete.lua` adds any aliases listed by `git config --get-regex alias` to the list of potential matches for git.
  
  NOTE: if you add new aliases, the command prompt must be reloaded.
* `git_branch_autocomplete.lua` pulls all branches (remotes included) at the time of autocomplete, provided that you're autocompleting `checkout`, `merge` or `rebase` (or a simple alias of one of those), and throws the branches in the match set.  As you type more of the branch name the autocomplete narrows.  

### Installation

These files should be placed in one of the following locations:

###### Windows XP
`c:\Documents and Settings\<username>\Local Settings\Application Data\clink`

###### Windows Vist or Later
`c:\Users\<username>\AppData\Local\clink`
