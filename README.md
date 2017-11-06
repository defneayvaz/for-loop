int w = 50;
int h = 50;
float mappedValue;
float mappedRad;
int multiplier = 1;

void setup() {

  size(600, 600);
}


void draw() {
  background(255);

  
  mappedValue = map(mouseX,0,width,0,255);
  fill(255,0,mappedValue,255);
  //println("mouseX: " + mouseX + "----" + "mappedValue: " + mappedValue);
  for(int i = 0; i < 10; i = i +1) {
   
  }
  
  
  //mappedRad = map(mouseX,0,600,0,600);
  
  
  if(mappedRad > 200) {
    multiplier = -1;
    println("greater than 200");
  }
  
  if(mappedRad < 0){
    multiplier = 1;
     println("lower than 0");
  }
  
  mappedRad = mappedRad + 1 * multiplier; 
  
  ellipse(200,200,mappedRad,mappedRad);
  rect(400,300,mappedRad,mappedRad);
   rect(400,400,mappedRad,mappedRad);
   rect(400,200,mappedRad,mappedRad);
   rect(400,100,mappedRad,mappedRad);
   rect(400,0,mappedRad,mappedRad);
   rect(100,400,mappedRad,mappedRad);
   rect(0,400,mappedRad,mappedRad);
   rect(200,400,mappedRad,mappedRad);
   rect(300,400,mappedRad,mappedRad);
   
   
  noStroke();
  //println(mappedRad);
  
  
  
  
  
  
  
  
}
