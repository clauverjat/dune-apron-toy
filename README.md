# Work in progress 

Goal : Make a simple ocaml executable link correctly with apron


Build and execute executable with 
```
dune clean
dune exec ./bin/main.exe
```

Current issue :
Runtime error :
`./bin/main.exe: symbol lookup error: ./bin/main.exe: undefined symbol: ap_policy_fprint`
