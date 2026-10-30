# >>> positpal auto-resume >>>
# Added by positpal::start() so capture picks up where you left off when you
# reopen this folder. Remove it with positpal::auto_resume(FALSE).
# positpal-store: ".capture"
# positpal-created-this-file
local({
  up <- path.expand("~/.Rprofile")
  if (file.exists(up) && !nzchar(Sys.getenv("POSITPAL_IN_USER_RPROFILE")) &&
      normalizePath(up) != normalizePath(".Rprofile")) {
    Sys.setenv(POSITPAL_IN_USER_RPROFILE = "1")
    on.exit(Sys.unsetenv("POSITPAL_IN_USER_RPROFILE"))
    source(up)
  }
})
if (interactive() && requireNamespace("positpal", quietly = TRUE) &&
    exists("resume", envir = asNamespace("positpal"), inherits = FALSE))
  try(positpal::resume(c(".capture", "/Users/coraliespakowski/Desktop/BIOL 343/BIOL343_CC5/.capture"), startup = TRUE, store = "20261029231731-5283b8b8"), silent = TRUE)
# <<< positpal auto-resume <<<
