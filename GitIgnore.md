## Create a .gitignore file:

```bash
#create .gitignore file
touch .gitignore

#create and write in .gitignore file
cat .gitignore
```

<br/>

## Content of .gitignore file:

- ### Ignore all .a files

```bash
\*.a
```

<br/>

- ### But do track lib.a, even though you're ignoring .a files above

```bash
!lib.a
```

<br/>

- ### Only ignore the TODO file in the current directory, not subdir/TODO

```bash
/TODO
```

<br/>

- ### Ignore all files in any directory named build

```bash
build/
```

<br/>

- ### Ignore doc/notes.txt, but not doc/server/arch.txt

```bash
doc/\*.txt
```

<br/>

- ### Ignore all .pdf files in the doc/ directory and any of its subdirectories

```bash
doc/\*_/_.pdf
```
