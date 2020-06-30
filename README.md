# cnv

hex -> decimal
decimal -> hex
decimal -> binary
...

converter


## vimscript integration

it can be integrated with vim with the following .vimrc:

```
:command! -nargs=0 Cnv :call Cnv()
function Cnv()
   let result = system("cnv " . expand("<cword>"))
   echo result
endfunction
```
