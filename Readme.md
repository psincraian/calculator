# Introduction
A very quick introduction to ANTLR4 and how to create an own language in an hour.
# How to run example
```
docker pull petrusqui/compiler
git clone git@github.com:psincraian/calculator.git
docker run -ti -v ~/Workspace/calculator:/data petrusqui/compiler:latest bash
cd /data
antlr Calculator.g4 -no-listener -visitor -o app
cp *.java app
javac app/*.java
cd app
java Run
```

And now write some equations to the console and press CTRL+D
```
a = 1+2
b = a^2
c = a + b * (a - 1)
a + b + c
```
