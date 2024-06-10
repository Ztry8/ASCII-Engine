# ASCII-Engine
## Tiny engine and C11 library for terminal graphics 
![screenshot](https://github.com/Ztry8/ASCII-Engine/blob/main/screenshots/1.PNG)

Engine based on SDL2.    
You need copy ```core.c``` and ```core.h``` files to your work directory.   
Written in VC, C11. Example code of main file:
```
#include "core.h"

unsigned char init_game() { return 0; }

void input_game(SDL_Scancode key) {}

void update_core(struct Core* core) {
	set_tile(core, '@', INDEX_YELLOW, 2, 0);
}

void shutdown_game() {}

int main(int argc, char* args[]) {
	struct Core core;
	if (init_core(&core) != 0) return 1;
	else run_core(&core);
	shutdown_core(&core);
	return 0;
}
```

### TODO:
#### Change color system
