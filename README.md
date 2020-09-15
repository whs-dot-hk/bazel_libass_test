```sh
$ bazel build @libass//:library
```

## Merge static libraries
```sh
$ mkdir test
$ find -L bazel-bin -type f \( -name *.a -not -path "**/copy_*/**" \) -exec cp '{}' test \;
$ cd test
$ for f in *.a; do ar -x f; done
$ rm -f *.a
$ ar -qc libass.a *.o
$ rm *.o
```
