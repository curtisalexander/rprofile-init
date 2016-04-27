

# devtools ============================
# recommended per Hadley Wickham
#   https://github.com/hadley/devtools#other-tips
# install packages from RStudio CRAN mirror
# ignore newlines when `browse()`ing
# give minimal output from `traceback()`
# automatically load devtools in interactive sessions
.First <- function() {
  options(
    repos = c(CRAN = "https://cran.rstudio.com/"),
    browserNLdisabled = TRUE,
    deparse.max.lines = 2)
}

if (interactive()) {
  suppressMessages(require(devtools))
}

# project root ========================
# recommended per Jenny Bryan
#   https://gist.github.com/jennybc/362f52446fe1ebc4c49f
RPROJ <- list(PROJHOME = normalizePath(getwd()))
attach(RPROJ)

cat("=====\n")
cat("sourcing project specific .Rprofile\n")
cat("retrieve the top-level project directory at any time with PROJHOME or via\n> get(\"PROJHOME\", \"RPROJ\")\n", get("PROJHOME", "RPROJ"), "\n\n")
cat("paths should be built like so:\n> file.path(PROJHOME, sub_dir, file_name)\n\n")
cat("for more details see the post at:\nhttps://gist.github.com/jennybc/362f52446fe1ebc4c49f\n")
cat("=====\n\n")
rm(RPROJ)
