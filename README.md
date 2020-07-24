# Trying to resolve github actions failures in R

For R v3.5.3 on Xenial Ubuntu I get failures using this workflow when building the package 'ff'. It's unclear exactly why this happens as when trying to recreate this with a vagrantbox I don't get similar failures.

I'll endeavour to troubleshoot in this repository.

This appears to be a corrupted package within Rstudio package manager for Ubuntu 16 for R 3.5.3 for the package 'ff'. Removing the rspm line in the build matrix resolves this.
