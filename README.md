# Fluxus-Movement-Code-Instructions-for-Computational-Art-
In the tradition of the Fluxus movement, in which instructions play a key role, I intended to make transparent the written, plain English instructions which guide the creation of computational art!

![judgey ducky](https://github.com/user-attachments/assets/d213014e-0c1f-42ea-a7d1-6a71cc14a2a2)

Intended output: A yellow, cartoon duck in a powerful stance against a purple background,  glaring at the viewer with a judgmental expression. A text box is near his head, which states what he is doing–scanning your vibe!
 
Library used: P5.js

Goals/influences: I was inspired by animated shorts I frequently see on social media. Lots of creatives make adorable, sassy characters, and there is a social media trend of cute animals "checking your vibe" as you scroll. It is often meant to be taken as a fun, positive break from doomscrolling. I also have some personal lore with stuffed animals with loved ones. One of my stuffed animals (definitely NOT influenced by my actions!) gets in a loved one's space to playfully assess their vibes. 
	
Feedback: A peer of mine wrote what he thought the instructions would be upon seeing the visual output, and assessed the efficacy of the code based on intended outcomes. You can check it out under feedback.md


Instruction: 

1.Set up the canvas

2.Create the background (P5.JS conventions so far!)

3.Draw the shadow for the duck 

4.Draw the duck's body using circles

5.Draw the duck head using circles

6.Draw the eye 

7.Draw the eye highlight

8.Draw the beak

9.Draw the judgmental eyebrow

10.Draw the feet far apart

11.Draw the legs to connect feet to body

12.Make the text box

13.Write out the text

14. Add missing details!

Instructions within code: 

			function setup() {
			createCanvas(600, 400);
			}
			function draw() {
	 		//color of background--light purple
			background(100, 100, 220);
			let s = "Duck Judge is scanning your vibe...";
			//shadow colors
			fill("#4929AE");
	  	noStroke();
	  	ellipse(200, 350, 250, 20);
	  	beginShape();
	  	vertex(383, 380, 10);
	  	vertex(298, 390);
	  	vertex(30, 360);
	  	vertex(280, 350);
	  	endShape(CLOSE);
	  	//color of ducky
	  	fill("yellow");
	  	//no outline needed...we want him chunky and the two circles to overlap
	  	noStroke(0);
	  	//ducky body. An ellipse allows for a wider shape
	  	ellipse(200, 210, 300, 260);
	  	//ducky head
	  	circle(220, 96, 130);
	  	circle(240, 95, 130);
	  	//color of ducky's eye
	  	fill("yellow");
	  	triangle(70, 120, 50, 200, 155, 90);
	  	fill("black");
	  	//i guess stroke makes sense here
	  	stroke("black");
	  	//the shape of the ducky's eye
	  	circle(220, 80, 20);
	  	//the light reflecting in Ducky's eye
	  	fill("white");
	  	noStroke;
	  	//it needs to be in the upper corner of the ducky's eye
	  	circle(218, 76, 10);
			//color of the beak
	  	fill("orange");
	  	//color of outline
	  	stroke("black");
	  	//shape of beak. xy,yy, xy2, yy2, etc. He needs to look judgey
	  	quad(280, 108, 382, 125, 320, 130, 225, 120);
	  	//the shape of the eyebrow. He needs to look very rude. He's a mean guy.
	  	noFill();
	  	strokeWeight(2);
	  	stroke(2);
	  	curve(200, 70, 204, 60, 245, 80, 215, 80);
	  	//the little line on his beak so he can huff and puff with tude
	  	line(287, 114, 289, 116);
	  	fill("#000000");
	  	//color of his feetz
	  	fill("orange");
	  	//color of outline
	  	stroke("black");
	  	beginShape();
	  	vertex(6, 360, 10);
	  	vertex(50, 340);
	  	vertex(30, 390);
	  	vertex(0, 390);
	  	vertex(0, 360);
	  	endShape(CLOSE);
	  	//color of his feetz
	  	fill("orange");
	  	//color of outline
	  	stroke("black");
	  	//the shape of his feetz
	  	beginShape();
	  	vertex(380, 390, 10);
	  	vertex(330, 384);
	  	vertex(300, 390);
	  	vertex(290, 350);
	  	endShape(CLOSE);
	  	//the lines connecting his feetz to his body
	  	line(50, 340, 89, 299);
	  	line(290, 350, 312, 298);
	  	//text box and font for the duck to judge you...
			fill("black");
		  rect(355, 70, 240, 40);
		  textSize(14);
		  fill("magenta");
		  strokeWeight(2);
		  text(s, 360, 100);
		  //shadows because it looks really flat
		  fill("#F1DC21");
		  //noStroke ();
		  arc(90, 180, 190, 110, 350, QUARTER_PI, OPEN, 300);
		  arc(90, 169, 200, 100, 111, QUARTER_PI);
		  arc(192, 120, 60, 20, 50, QUARTER_PI);
		  fill("#A27A01");
		  beginShape();
		  vertex(13, 370);
		  vertex(15, 385);
		  vertex(30, 365);
		  vertex(40, 345);
		  endShape();
		  beginShape();
		  vertex(309, 375);
		  vertex(320, 380);
		  vertex(309, 368);
		  endShape();
		}
check out the drawing here: https://editor.p5js.org/Kmorrissey1/sketches/h35NQ0x18
