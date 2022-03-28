Command I used:

```
conan install "C:\dev\conan_issue_10900" --install-folder "C:\dev\conan_issue_10900\build" --output-folder "C:\dev\conan_issue_10900\build" --profile:host test-profile --profile:build test-profile -s build_type=Release -s arch=x86_64
```

### Expected:

sh scripts in C:\dev\conan_issue_10900\build\conan


### Actual results:

```
$ ls -l /c/dev/conan_issue_10900/build/build/conan/
total 11
-rw-r--r-- 1 walid 197121 2634 Mar 28 14:41 conan_toolchain.cmake
-rw-r--r-- 1 walid 197121  102 Mar 28 14:41 conanbuild.conf
-rw-r--r-- 1 walid 197121   91 Mar 28 14:41 conanrun.bat
-rw-r--r-- 1 walid 197121  904 Mar 28 14:41 conanrunenv-release-x86_64.bat
-rw-r--r-- 1 walid 197121  102 Mar 28 14:41 deactivate_conanrun.bat
```