# vim-syntax-extra

> This plugin is basically the copy of ['justinmk/vim-syntax-extra'](https://github.com/justinmk/vim-syntax-extra)    
> I copy it for some personalized changes.  
> For more information, please refer to the page above.
---
## Things I customized:
1. Add 
```vim
syn match cType "\v[A-Z][a-z0-9]+" 
```
  to the first line of c.vim to highlight the words start with captical letter.
 Thus, the `Node` below will be highlighted.
  ```c
  typedef struct Node Node
  Node{
    int value;
    Node *next;
  };
  ```
---
2. Remove `cType` in following line
 ```vim
 syn match cUserFunction "\<\h\w*\>\(\s\|\n\)*("me=e-1 contains=cType,cDelimiter,cDefine
 ```
 in c.vim
 for not overwriting the highlight of user defined function.

---
3. Make comments and strings in c italicized.  
  

