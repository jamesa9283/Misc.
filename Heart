float [] x = new float [100];
float [] y = new float [100];

void setup() {
  size(600,600);
  strokeWeight(5);
  stroke(255,0,0);
}

void draw() {
  translate(width/2,3*height/4);
  background(255);
  for (int i=0; i<610; i++) {
    x[i] = 0.1 * (-pow(i,2) + 60*i + 1200)*sin((PI*i)/180);
    // move the end elements down 1
    arraycopy(x, 100, x, 99, x.length-100);
// remove the extra copy of the last element
    x = shorten(x);
    y[i] = -0.1 * (-pow(i,2) + 60*i + 1200)*cos((PI*i)/180);
    // move the end elements down 1
    arraycopy(y, 100, y, 99, y.length-100);
// remove the extra copy of the last element
    y = shorten(y);
    
    point(x[i],y[i]); // use these to place your little hearts
    point(-x[i],y[i]); // use these to place your little hearts
    endShape();
  }
}
