	<h4>Relative Velocity</h4>

	<h4>Project Directory Structure  </h4>

This project contains files and folders. The structure of the contents of this  folder is outlined below:<br>  
	images/  <br> 
This contains any images used for instruction showing, canvas images, arrow ‘s images for changing angle. <br> 
	js/  <br> 
This contains the JavaScript files used.   Jquery and the bootstrap is used by the project. <br>  
	css /<br> 
 Style Sheets for this project. Here includes the css files which is given with the bootstrap<br>  

	bootstrap.css<br> 
	bootstrap.min.css<br> 
	bootstrap-theme.css<br> 
	bootstrap-theme.min.css<br> 
	font-awesome.min<br> 

	<h4>Index.html</h4>
The index.html file contains all main functionality functions used in this project.
These are defined with several method and variables, explained below.
	
	<h5>Variables</h5>
Flag:indicate the current case. 1 or case 2<br>
	case 1 varibles<br>
	vo:object velocity  <br>
rvo:relativity of velocity <br>
rvog: relative velocity of object relative to ground <br>
	rvor: relative velocity of object relative to river <br>
	deg:degree that given by user<br>
	edge:degree value of relative to earth/river<br>
	cdeg:degree to draw curve<br>
	vr:velocity of river <br>
	wr:width of river<br>
	ct:crossing time<br>
	cd:crossing distance<br>
	dd:distance of go down to the river<br>
	dd2: distance of go up to the river<br><br>
	
for drawings temporary variables <br>
	tvo1: temporary velocity for animation<br>
	tvo2: temporary velocity for animation<br>
	c:counter for animation(for timer)<br>
	sh: temporary canvas height<br>
	r_deg:radius of radian<br>
	angleInDegrees: drawing arrow in case 1<br><br>
	
	
case 2 varibles<br>
b1v:object 1 velocity<br>
	b2v: object 2 velocity<br>
	b1deg:object 1 bearing<br>
	b2deg:object 2 bearing<br>
	dist:distance between object<br>
	distdeg:bearing of object 2 relative to object 1<br>
	b1rv:object 1 relative velocity<br>
	b2rv:object 2 relative velocity<br>
	shortd:shortest distance if available<br>
	time:time taken to obtain shortest distance<br>
bd1:distance  from start position of object 1 when shortest distance <br>
bd2: distance from start position  object 1 when shortest distance<br>
b1deg2:bearing of object 1 when shortest distance <br>
b2deg2:bearing of object 2 when shortest distance <br>
angleInDegrees2:drawing arrow in case 2 first object<br>
angleInDegrees3:drawing arrow in case 2 second object<br>
type: "M" for meet "S" for shortest distance "N" for no shortest distance<br><br>
	
	for drawings temporary variables<br>
	tvb1n:object one velocity to north<br>
	tvb1e :object one velocity to east<br>
	tvb2n::object 2 velocity to north<br>
	tvb2e:object 2 velocity to east<br>
	pix:minimum pixels between objects<br>
reldist1:relative distance when shortest available<br>
reldist2:relative distance when shortest available<br>

	<h4>Methods</h4>
Setflag:switch between  case 1 and case 2<br>

Case 1 methods<br>
drawObject:draw the boat object<br>
arrow:draw the rotated arrow when rotating<br>
includes the mouseclick,mouse moving, drawRotated method.Both object and arrow will draw by this method.<br>


Arrowchng: This method works when fill angle in the form and draw the arrow according to given value<br>

Cal: calculations are done here.all the velocities,times,angle will calculated.<br>

Reset:last drawed image will delete.useful for do the simulations again and again<br>

Cl:object drawed in start position.useful for do the simulations again and again<br>

Move: for animate the object acoording to velocity<br>

Stop: stop the animation<br>

Ruler: for drawing the ruler in canvas.help to see the scaling<br>

Showdata: calculated data will show using this method<br>

Confirmbtnshow: to show the confirm button in the popup form to validate data<br>

Submitbtnshow:if data are validated ok button will show<br>

Chng: change the canvas heigh.for showing the movements which cannot show with current canvas height<br>

Animateshow:show the animate button after click the ok button in the popup form<br>

Animatehide: hide the animate button <br>

Case 2 methods<br>

drawObject:call this to draw the one boat object when needed <br>

arrow: draw the rotated arrow when rotating.includes the mouseclick,mouse moving, drawRotated method.<br>

Caldata:to calculate velocities ,time and other data need to show.<br>

Setvariables: calculate temp velocities for drawing<br>

Taketostart:determine and draw start position of objects<br>

move2:animations starting<br>

stop:stop animations<br>

animateshow:show the animate button to start simulations<br>

confirmbtnshow:to show confirm button for validate data  in the popup form<br>

submitbtnshow:to ok button after validating data in the popup form<br>

chngarrow1,/chngarrow2:to change arrow when changing bearing values of boat 1/boat 2 in the form<br>
 
