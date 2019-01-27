function setup() {
    createCanvas(600, 600);
}

function draw() {
    background(51);
}

function Ship() {
	this.x = width/2;

	this.show = function() {
		fill(255);
		rectMode(CENTER);
		rect(this.x, height-20, 20, 60);
	}

	this.move = function(dir) {
		this.x += dir*5;
	}
}

var ship;

function setup() {
	createCanvas(600, 400);
	ship = new Ship();
}

function draw() {
	background(51);
	ship.show();
	}

}

 function keyPressed() {
	if (keyCode === RIGHT_ARROW) {
		ship.move(1);
	} else if (keyCode === LEFT_ARROW) {
	  ship.move(-1);
	}
}
