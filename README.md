# snippet-stash.nvim

**snippet-stash.nvim** is a neovim plugin for storing code blocks for usage/insertion later. can be used as a fancy clipboard or just a supplement to in-line snippets. code blocks are only stored per filetype.

after using neovim for about 5 years, this is my first time making a plugin.

## installation

### using [`lazy.nvim`](https://lazy.folke.io/installation)

```lua
{
 'akfiveseven/snippet-stash.nvim',
  config = function()
    require('snippet-stash').setup()
  end
}
```

### manual installation

1. copy `snippet-stash.lua` into the `lua` folder of your config
2. add `require('snippet-stash').setup()` in your `init.lua` file
3. restart neovim
4. try the `:SnippetList` command to verify its installation

## commands

- use `:SnippetSave` in visual mode to save a code block and label it
- use `:SnippetShow` to open the snippet menu and select a snippet to insert
- use `:SnippetDelete` to open the snippet menu and delete a snippet
- use `:SnippetList` to simply print the snippet list to standard output


