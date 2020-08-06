# snapshot

You have some tasks that take a long time to complete, so you want to run them in parallel.

Snapshot uses Git to manage multiple isolated changes in parallel.

# Usage

Make your changes, then with the long running task, run:

```
snapshot packer run ....
```

Snapshot will:

* create a branch for your changes
* run the changes in the background
* reset your git to what was committed to master

You can now make another set of isolated set of changes to test out.

To see running builds, run:

```
snapshot status
```

To attach to a running build, run:

```
snapshot attach
```

