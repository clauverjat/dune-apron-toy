A simple example of an executable using libapron.

Build and execute executable with 
```
dune clean
dune exec ./bin/main.exe
```

It should print something like that :
```
Using Library: polka, strict mode, version 3.0 with NUMINT_MPZ
env=[|0> w:int; 1> x:int; 2> y:int; 3> z:int; 4> a:real; 5> b:real;
      6> u:real; 7> v:real|]
env2=[|0> w:int; 1> x:int; 2> y:int; 3> z:int|]
tab = [|1/2x+2/3y+1=0; -2.w-z+4.>=0; 2.w+z+[-2.; -1.]>=0; u>=0; -u+5>=0|]
abs=[|3x+4y+6=0; -2w-z+4>=0; -u+5>=0; u>=0; 2w+z-1>=0|]
gen=[|LIN:-w+2z; LIN:-4x+3y; LIN:v; LIN:b; LIN:a; VTX:1/2w-2x;
      VTX:1/2w-2x+5u; VTX:2w-2x; VTX:2w-2x+5u|]
gen=[|LIN:-w+2z; LIN:-4x+3y; LIN:v; LIN:b; LIN:a; VTX:1/2w-2x;
      VTX:1/2w-2x+5u; VTX:2w-2x; VTX:2w-2x+5u|]
box=[|[-1/0; 1/0]; [-1/0; 1/0]; [-1/0; 1/0]; [-1/0; 1/0]; [-1/0; 1/0];
      [-1/0; 1/0]; [0; 5]; [-1/0; 1/0]|]
Bound of 1/2x+2/3y+1 = [0; 0]
Bound of -2.w-z+4. = [0; 3]
Bound of 2.w+z+[-2.; -1.] = [-1; 3]
Bound of u = [0; 5]
Bound of -u+5 = [0; 5]
abs2=[|-a+5>=0; a>=0|]
abs3=bottom
is_bottom(abs3)=true
abs=[|3x+4y+6=0; -2w-z+4>=0; -u+5>=0; u>=0; 2w+z-1>=0|]
p2=expand(abs,y,[y1,y2]))=[|3x+4y2+6=0; 3x+4y1+6=0; 3x+4y+6=0; -2w-z+4>=0;
                            -u+5>=0; u>=0; 2w+z-1>=0|]
p2=expand(abs,u,[u1,u2]))=[|3x+4y+6=0; -2w-z+4>=0; -u+5>=0; -u1+5>=0;
                            -u2+5>=0; u2>=0; u1>=0; u>=0; 2w+z-1>=0|]
Using Library: oct, version 1.0 with NUM_MPQ
env=[|0> w:int; 1> x:int; 2> y:int; 3> z:int; 4> a:real; 5> b:real;
      6> u:real; 7> v:real|]
env2=[|0> w:int; 1> x:int; 2> y:int; 3> z:int|]
tab = [|1/2x+2/3y+1=0; -2.w-z+4.>=0; 2.w+z+[-2.; -1.]>=0; u>=0; -u+5>=0|]
abs=[|u>=0; -u+5>=0|]
gen=[|VTX:0; LIN:w; LIN:x; LIN:y; LIN:z; LIN:a; LIN:b; LIN:u; LIN:v|]
gen=[|VTX:0; LIN:w; LIN:x; LIN:y; LIN:z; LIN:a; LIN:b; LIN:u; LIN:v|]
box=[|[-1/0; 1/0]; [-1/0; 1/0]; [-1/0; 1/0]; [-1/0; 1/0]; [-1/0; 1/0];
      [-1/0; 1/0]; [0; 5]; [-1/0; 1/0]|]
Bound of 1/2x+2/3y+1 = [-1/0; 1/0]
Bound of -2.w-z+4. = [-1/0; 1/0]
Bound of 2.w+z+[-2.; -1.] = [-1/0; 1/0]
Bound of u = [0; 5]
Bound of -u+5 = [0; 5]
abs2=[|a>=0; -a+5>=0|]
abs3=bottom
is_bottom(abs3)=true
abs=[|u>=0; -u+5>=0|]
p2=expand(abs,y,[y1,y2]))=[|u>=0; -u+5>=0|]
p2=expand(abs,u,[u1,u2]))=[|u>=0; -u+5>=0; -u+u1+5>=0; u+u1>=0; u1>=0;
                            -u-u1+10>=0; u-u1+5>=0; -u1+5>=0; -u+u2+5>=0;
                            u+u2>=0; -u1+u2+5>=0; u1+u2>=0; u2>=0;
                            -u-u2+10>=0; u-u2+5>=0; -u1-u2+10>=0; u1-u2+5>=0;
                            -u2+5>=0|]
```
