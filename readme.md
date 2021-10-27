BPGP Maven aggregator project
=============================
Used to develop BPGP-context together with
- BPjs-Context
- BPjs

Instructions
------------
- `git clone` the directories, as siblings of this
- modify each `pom.xml` `version` tag to contain `-SNAPSHOT`
- modify BPGP-context' `pom.xml` to use the `-SNAPSHOT` versions
- comment out the `itpack.io` `repository` section in BPGP-context' `pom.xml`, as it interferes
- maybe need to lowercase BPjs-Context's `groupId`
- IntelliJ, optional:
    - Ctrl-Shift-A -> Delegate IDE build/run actions to Maven -> (enable)
        - easier for debugging compilation problems; but worse on running phase...
    - You might also want to "Skip Tests" at the same Maven-Runner dialog
    - and also add a property ("+" icon beneath it: `maven.javadoc.skip` value `true`)