# elArt
Pixel Art demo framework.

## Purpose
ElArt will kickstart your Pixel Art experiments by wrapping off-screen rendering
backend into easy-to-setup package, targetted directly at spitting pretty pixels.

```
#include "elArt.tbasicu"

function tbMain()
    
  dim art as elArt  
  art.createCanvas("Cloudy evening - press ESC to quit", 1280, 720, 180, 90)
         
  ' -- Main loop
  while art.HasCanvas    
    art.beginDrawing   
      ' -- draw something here     
    art.endDrawing

    if art.keyDown(%VK_ESCAPE) then exit while
  wend

  art.destroyCanvas
end function
```
