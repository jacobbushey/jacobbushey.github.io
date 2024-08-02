---
layout: default
title: Tips for the cluster
# permalink: /coding-tips/cluster/
---

## Tips for the cluster

If a user's name was John Harvard:

### unix/ bash
- `rsync`: move files from local drive to remote
- `find . -exec touch {} \;`: touch all files within a directory 
- 'scp source_filepath/filename jharvard@login.rc.fas.harvard.edu:destination:filepath': from your local machine, moves a file onto the cluster. Use the recursive flag to move multiple files, reverse the order of the arguments to move files from the cluster to your home machine.

### slurm
- `salloc`: starts an interactive job
- `sshare`: prints fairshare score

#### slurm flags 
- `-p` controls partition (eg. huce_cascade, huce_intel)
- `-c` controls cpus per task 
- `-m` minimum memory per core
- `-d` controls dependencies
- '-r' makes the argument recursive
