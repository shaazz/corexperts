function show(){
  //create a div
  var logo = document.createElement('div');
	logo.style.width="300px";
	logo.style.height = "80px";
	logo.style.overflow = "hidden"
	//create a paragraph
  var p1 = document.createElement('p');
	p1.style.fontSize = "20pt";
	p1.innerHTML = "Core"
	p1.style.fontWeight = "bold"
	p1.style.cssFloat = "left";
	//create a para 2
	var p2 = document.createElement('p');
	p2.style.fontSize = "50pt";
	p2.innerHTML = "X"
	p2.style.fontWeight = "bold"
	p2.style.cssFloat = "left";
	p2.style.marginTop = "10px"
  //create transition for animation how much time X running
	p2.style.transition =  "all 60s";
	p2.style.cursor = "pointer"

  //create para 3
	var p3 = document.createElement('p');
	p3.style.fontSize = "20pt";
	p3.innerHTML = "perts"
	p3.style.fontWeight = "bold"
	p3.style.cssFloat = "left";
	//create transformation of X
	function ani(){
				p2.style.transform = "rotateY(7200deg)"
		}
	//for delay X Animation  
window.setTimeout(ani,1);

// all paragraph append in div 
	logo.appendChild(p1);
	logo.appendChild(p2);
	logo.appendChild(p3);

var bodies = document.body
//div append in body for showing web
bodies.appendChild(logo);	



	}

window.addEventListener('load',show);	
