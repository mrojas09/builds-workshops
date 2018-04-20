Lab08: Revenge of Lab03

You can experiment with the functions by running `cabal repl` in this directory.

```
:add Example
*Example> AstInt 2
AstInt 2
*Example> AstInt (- 4444)
AstInt (-4444)
*Example> AstPlus (AstInt 1) (AstInt 1)
AstPlus (AstInt 1) (AstInt 1)
*Example> AstInt "seven"

<interactive>:7:8: error:
    * Couldn't match expected type `Integer' with actual type `[Char]'
    * In the first argument of `AstInt', namely `"seven"'
      In the expression: AstInt "seven"
      In an equation for `it': it = AstInt "seven"
      
      
*Example> eval (AstPlus (AstInt 2) (AstInt 3))
5
*Example> eval (AstPlus (AstInt 4) (AstPlus (AstInt 2) (AstInt 3)))
9

```

