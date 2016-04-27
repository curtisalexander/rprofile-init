# rprofile-init
Initialize a project specific `.Rprofile` within a directory based on the `rproject-init/Rprofile` file.

### Customize 
Update the file `Rprofile` within the `rprofile-init` directory to your liking.

### Usage
Within an R project directory, create an `.Rprofile` file.  I prefer to symlink `rproject-init` into `~/bin` which is on my `$PATH`.  To use, `cd` into the directory desired and run the script.

```bash
cd ~/projects/awesome-r-analyis
rproject-init
```

### Questions
**Q:** Why not just use a global `~/.Rprofile`?

**A:** When using [packrat](rstudio.github.io/packrat/) as part of an R project, `packrat` automatically creates an `.Rprofile` file within the project directory.  Running `rprofile-init` copies the `rprofile-init/Rprofile` file into the local `.Rprofile` file, thus adding custom content to an already created `.Rprofile` file.
