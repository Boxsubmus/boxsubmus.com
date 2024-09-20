+++
title = 'Trinket'
+++

<img src="/trinket_icon.svg" style="width:64px; margin-right: 16px" align="left">

Trinket is a [libreware](https://www.libreware.org) 2D game engine designed for ease of use and modification. Unlike most modern engines today, Trinket is designed with a focus on developer productivity instead of 'bloatware features' or 'beginner accessibility'.

<br>
The Trinket IDE allows you to make games in a fraction of the time it would take to start from scratch, featuring everything you need to view and modify the assets of your game.

![alt text](/screenshot1.png)

Using the [Beef Programming Language](https://www.beeflang.org/) and IDE, you can quickly script and debug your game.

![alt text](/screenshot2.png)

## Design Goals
* High performance execution
* A compiled programming language as the main form of scripting
* Easy to modify API
* Multi-platform (Consoles, PC, Android)
* Actual decent audio support
* IDE designed for productivity
  * Not made from a web browser
  * No tracking or analytics
  * No installer or forced updates
  * Near-instant hot-loading for almost every type of asset

## Examples:

**C++ Scripting:**
```cpp
#include "Trinket/Scripting/Object.hpp"
#include "Trinket/Dev/Log.hpp"

using namespace Trinket;

namespace GameLogic
{
    class PlayerObject : public Object
    {
    public:
        void CreateEvent() override
        {
            Debug::Log("Hello!");
        }
    };

    TRINKET_REGISTER_OBJECT(PlayerObject);
}
```

#### Trinket is currently a work-in-progress, please stay tuned for updates!