# potroshitel_sdk ![CS:GO](https://img.shields.io/badge/game-CS%3AGO-orange?style=flat) ![LANG](https://img.shields.io/badge/language-C%2B%2B-brightgreen?style=flat )
a clean sdk which has everything you need for a fully featured internal cheat

# features
- engine_prediction ( but not fully )
- bhop
- movement fix

# other
- easy to use n understand project structure & code

# hooks
- reset
- present
- lock_cursor
- create_move

# conventions
prefix classes with 'c_', interfaces classes with 'i', enums with 'e_' and postfix structures with '_t'
```cpp
class c_class;
class i_interface;
struct struct_t;
enum e_enum;
```

## requirements
- [dx sdk](https://www.microsoft.com/en-us/download/details.aspx?id=6812)
- [c++ redists ( optional )](https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads)

# credits
 - [imgui](https://github.com/ocornut/imgui)
 - [vmt](https://github.com/gfreivasc/VMTHook)
 
 # code style example
```cpp
struct some_struct_t {
    bool m_some_shit;
};

class c_some_class {
public:
    bool m_some_shit;
};

enum e_some_enum {
    SOME_SHIT
};

void c_self_class::test_func() {
    const auto local = globals::m_local
    static const auto setup_bones_sig = SIG("client.dll", "55 8B EC 83 E4 F0 B8 D8").cast<void**>();
}
```