# processingEx
yoyo

this is the example

void setup(){
  size(1260, 680);
  
}
  int bgR = 0;
  int bgG = 0;
  int bgB = 0; 
  int bgRcheck = 0;
  int bgGcheck = 0;
  int bgBcheck = 0;
  
void draw(){
  backgroundStuff();
  background(bgR);
  //background(bgR,bgG,bgB); <---- this is colour(ed) mode..
}


 
void backgroundStuff(){
  if(bgR <= 255 && bgRcheck == 0){
    bgR++;  
    if(bgR == 254){
      bgRcheck = 1;
    }
  }
  if(bgG <= 255 && bgGcheck == 0){
    bgG++;  
     if(bgG == 254){
      bgGcheck = 1;
    }
  }
  if(bgB <= 150 && bgBcheck == 0){
    bgB++;
    if(bgB == 254){
      bgBcheck = 1;
    }
  }
  if(bgR >= 20 && bgRcheck == 1){
    bgR--;  
     if(bgR <= 20){
      bgRcheck = 0;
    }
  }
  if(bgG >= 20 && bgGcheck == 1){
    bgG++;  
    if(bgG <= 20){
    bgGcheck = 0;
    }
  }
  if(bgB >= 20 && bgBcheck == 1){
    bgB--;
    if(bgB <= 20){
    bgBcheck = 0;
    }
  }
}
