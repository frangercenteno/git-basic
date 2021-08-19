# Git Comandos Básicos

## Concepts

Git is a Version Control System to register our changes to a file or set of files.

![Version Control](https://blog.cpanel.com/wp-content/uploads/2018/05/image2018-2-8_17-46-1.png)

---

## States

1. Working Directory
    - Here is where edit and work our project.

2. Staging Area
    - Here is where we select the files that are ready to go to third state, just as we decide which files are not ready.

3. Repository
    - Here is where we to register all our project.

![Git State](https://git-scm.com/figures/18333fig0106-tn.png)

---

## Configuration

### __*User*__

```bash
	$ git config --global user.name "username"`
```

### __*Email*__


```bash
	$ git config --global user.email "username@domian.com"
```

### __*See global configuration*__


```bash
	$ git config --global -l
```

---

## Create repository

```bash
	$ git init
```
---

## Know status

- If exist files with red color, it means that they have not been added to change control (___Working Directory___) or your are not having a control.

```bash
	$ git status
```
---

## Add filles and prepare it to the ___staging___ 

- When typing the command `$ git add ` and add a __*"."*__ to finish, all change will be added, but if you want to add a specific file, just type its name.

- All files in a directory can be added with the next command.

```bash
	$ git add src/
	$ git add src/*.js
	$ git add */*.js
	$ git add .
```

---

## Add files to ___staging___  (commit)

```bash
	$ git commit -m "commit message"
```
- The command "m" representing to command to write a message.

---
## See differences in changes made to files before ___staging__

```bash
	$ git diff
```

---

## Remove change before ___staging___

```bash
	$ git checkout .
```
---
## See change history

```bash
	$ git log	
```

---

## Remove added files for uploading to __stage__

```bash
	$ git reset filename.example
```

---

## Help command
### See all command definitions

```bash
	$ git help
```

- We can see a specific command with next command. Example `commit`.

```bash
	$ git help specific_command
```

---

## Add alias to commands

- Add alias to be more specific when write commands.

- A command example is ___log___.

```bash
  $ git config --global alias.l "log"
```
- Result

```bash
	$ git l
```

---

## Change or modify a commit message

```bash
	$ git commit --amend -m "mensagge"
```

## Rename a file created after a  ___commit___

```bash
	$ git mv oldname.html newname.html
```

---

## Delete a file after commit

```bash
	$ git rm newname.hmtl
```

---

## Rollback a previous commit

```bash
	$ git reset --hard idcommit
```

---
