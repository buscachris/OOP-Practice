# C++ object-oriented programming practice

I wrote three small programs to see which function C++ calls when names are shared across overloads or across a class hierarchy.

| Example | What I show |
| --- | --- |
| [Overloads and overrides](Function-overload-overriding.cpp) | I call overloaded `test` functions with different argument types and use a virtual `Display` method in a base and derived class. |
| [Method hiding](MethodOverriding++/main.cpp) | I call `disp` on a derived object. Both classes declare a nonvirtual method with that name. |
| [Static and dynamic binding](Static-VS-Dynamic/main.cpp) | I call a virtual method through a base pointer, then select a `sum` overload by passing two or three arguments. |

I build each example separately because each file defines its own `main`. From the repository root I use the following commands.

```sh
c++ Static-VS-Dynamic/main.cpp -o /tmp/binding-demo
/tmp/binding-demo
```

## License

I license my C++ examples and accompanying notes under the [MIT License](LICENSE).
