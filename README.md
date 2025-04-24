# Description
Search using grep and an optional globbing pattern - inspired by teej-dv telescope video https://www.youtube.com/watch?v=xdXE1tOT-qg&t=153s 

globbing pattern is inserted after 2 spaces

for example:
`whatever I'm searching for  *.cs`
`whatever I'm searching for  **/test/**`

# Configuration

## Lazy Nvim
This is my lazy configuration with example bindings

```lua
return {
  'Dreagen/search-with-globbing.nvim',
  name = 'search-with-globbing',
  keys = {
    {
      '<leader>sg',
      '<cmd>lua require("search-with-globbing").search_with_globbing()<CR>',
      mode = { 'n', 'o', 'x' },
      desc = 'Search with Globbing',
    },
  },
}
```
