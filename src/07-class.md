# Classes & Objects

A C++ class is an user-defined data type that may contain it's own unique methods, attributes, etc. 
To define your own class, use the `class` keyword along with a useful name for it. 

We will be defining our own class, and use it to describe the next sections: 

```c++
#include<strings>
class Summon{
    // Class attributes
    std::string name; 
    char type; 
    int tier; 
    std::string description; 

    // Constructor 
    Summon(std::string name, char type, int tier, std::string description); 

    //Private Methods:
    private:
    int what_dmg(Summon s){ //Finds dmg of a perticular summon
        if s.type == 'T'{
            return (s.tier * 2 ) - 1; 
        } else if s.type == 'S' {
            return s.tier * 2;
        } else {
            return 0;
        }
    }

    //Public Methods: 
    public: 
    void info(Summon s){
        std::cout << 
    }
};

```