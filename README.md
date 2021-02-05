## twitter001 | #つぶやきProcessing 
https://twitter.com/nicolasbaez/status/1225237090662834176?s=20

![twitter](https://github.com/nicolasbaez/twitter001/blob/master/twitter001.gif)
```processing
void setup() { 
  size(512, 256);
} 
int k=0; 
int w=512; 
int h=256; 
void draw() { 
  background(0); 
  for (int i=0; i<w; i+=3) { 
    stroke(255); 
    line(i, map(sin(radians(map(i+k, 0, w, 0, 360*4)))+cos(radians(map(i*0.5+k, 0, w, 0, 360*4))), -2, 2, h, h/2), map(i, 0, w, w*0.5, w), 0);
  } 
  k+=1;
}
````
