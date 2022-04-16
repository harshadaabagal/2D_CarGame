--
Install PYCharm Editor.
Install package pygame.

Main Inbuilt functions:-

import pygame - This provides access to the pygame framework and imports all functions of pygame.

pygame.init() - This is used to initialize all the required module of the pygame.

pygame.display.set_mode((width, height)) - This is used to display a window of the desired size. The return value is a Surface object which is the object where we will perform graphical operations.

pygame.event.get()- This is used to empty the event queue. If we do not call this, the window messages will start to pile up and, the game will become unresponsive in the opinion of the operating system.

pygame.QUIT - This is used to terminate the event when we click on the close button at the corner of the window.

pygame.display.flip() - Pygame is double-buffered, so this shifts the buffers. It is essential to call this function in order to make any updates that you make on the game screen to make visible.

Pygame Blit
The pygame blit is the process to render the game object onto the surface, and this process is called blitting. When we create the game object, we need to render it. If we don't render the game objects and run the program, then it will give the black window as an output.

Blitting is one of the slowest operations in any game so, we need to be careful to not to blit much onto the screen in every frame. The primary function used in blitting is blit(), which is:

blit()

blit(source,dest,area=None,special_flags=0)  
gd.blit(render, (x_pos,y_pos))

Pygame Adding Image
To add an image on the window, first, we need to instantiate a blank surface by calling the Surface constructor with a width and height tuple.

surface = pygame.Surface((100,100))  
The above line creates a blank 24-bit RGB image that's 100*100 pixels with the default black color.

Pygame Keydown
Pygame KEYDOWN and KEYUP detect the event if a key is physically pressed and released. KEYDOWN detects the key press and, KEYUP detects the key release. Both events (Key press and Key release) have two attributes which are the following:

key: Key is an integer id which represents every key on the keyword.
mod: This is a bitmask of all the modifier keys that were in the pressed state when the event occurred.