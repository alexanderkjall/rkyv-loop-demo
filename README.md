```
$ cargo build
error: cyclic package dependency: package `borsh v1.6.0` depends on itself. Cycle:
package `borsh v1.6.0`
    ... which satisfies dependency `borsh = "^1"` (locked to 1.6.0) of package `uuid v1.21.0`
    ... which satisfies dependency `uuid = "^1.1.2"` (locked to 1.21.0) of package `bson v2.15.0`
    ... which satisfies dependency `bson = "^2"` of package `borsh v1.6.0`
```
