```
$ cargo build
error: cyclic package dependency: package `uuid v1.21.0` depends on itself. Cycle:
package `uuid v1.21.0`
    ... which satisfies dependency `uuid = "^1.1.2"` (locked to 1.21.0) of package `bson v2.15.0`
    ... which satisfies dependency `bson = "^2"` of package `borsh v1.6.0`
    ... which satisfies dependency `borsh = "^1"` (locked to 1.6.0) of package `uuid v1.21.0`
    ... which satisfies dependency `uuid = "^1.3"` (locked to 1.21.0) of package `rkyv v0.7.46`
    ... which satisfies dependency `rkyv = "^0.7"` (locked to 0.7.46) of package `num-complex v0.4.6`
    ... which satisfies dependency `num-complex = "^0.4.0"` (locked to 0.4.6) of package `approx v0.5.1`
```
