# R automatically runs an .Rprofile script (if present) each time RStudio opens a project.
#
# This R script sets one Git option for this repository only: pull.rebase = false.  
# Without that, Git on a Mac aborts a pull:
#   fatal: Need to specify how to reconcile divergent branches.
# Turning off rebasing (an advanced Git feature) allows Git to auto-merge "resolvable" conflicts.

try(suppressMessages(usethis::use_git_config(scope = "project", pull.rebase = "false")), silent = TRUE)

# usethis::use_git_config() is the same function you used in the Github_Workflow worksheet to set your name and email.  
# suppressMessages() and try(..., silent = TRUE) keep any messages from printing when this script runs.  
