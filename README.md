Данная лабораторная работа посвещена изучению инструментов статического и динамического анализа кода
```ShellSession
$ open http://cppcheck.sourceforge.net
```

## Tasks

- [x] 1. Ознакомиться со ссылками учебного материала
- [x] 2. Используя **cpplint** провести анализ проекта на **C++**
- [x] 3. Используя **Cppcheck** провести анализ проекта на **C++**
- [x] 4. Используя **OCLint** провести анализ проекта на **C++**
- [x] 5. Используя **Valgrind** провести анализ проекта на **C++**
- [x] 6. Составить отчет и отправить ссылку личным сообщением в **Slack**

```ShellSession

$ cpplint main.cpp
Done processing main.cpp
```

```ShellSession
$ cppcheck main.cpp
Checking main.cpp...
```

```ShellSession
$ oclint main.cpp -- -c

OCLint Report

Summary: TotalFiles=1 FilesWithViolations=0 P1=0 P2=0 P3=0 


[OCLint (http://oclint.org) v0.13]
```

```ShellSession
$ valgrind ./main
==4136== Memcheck, a memory error detector
==4136== Copyright (C) 2002-2015, and GNU GPL'd, by Julian Seward et al.
==4136== Using Valgrind-3.11.0 and LibVEX; rerun with -h for copyright info
==4136== Command: ./main
==4136== 
Hello, world!
==4136== 
==4136== HEAP SUMMARY:
==4136==     in use at exit: 72,704 bytes in 1 blocks
==4136==   total heap usage: 2 allocs, 1 frees, 73,728 bytes allocated
==4136== 
==4136== LEAK SUMMARY:
==4136==    definitely lost: 0 bytes in 0 blocks
==4136==    indirectly lost: 0 bytes in 0 blocks
==4136==      possibly lost: 0 bytes in 0 blocks
==4136==    still reachable: 72,704 bytes in 1 blocks
==4136==         suppressed: 0 bytes in 0 blocks
==4136== Rerun with --leak-check=full to see details of leaked memory
==4136== 
==4136== For counts of detected and suppressed errors, rerun with: -v
==4136== ERROR SUMMARY: 0 errors from 0 contexts (suppressed: 0 from 0)
```

## Links

- [Google C++ Style Guide](https://github.com/cpplint/cpplint)
- [Cppcheck Manual](http://cppcheck.sourceforge.net/manual.pdf)
- [Valgrind Quick Start Guide](http://valgrind.org/docs/manual/index.html)
- [OCLint Tutorial](http://docs.oclint.org/en/stable/intro/tutorial.html)

```
Copyright (c) 2017 Братья Вершинины
```
