var result = document.getElementById("result");
 var buttons = document.querySelectorAll("button")
 var screen = ""
 
for(index of buttons){
  index.addEventListener('click',(e)=>{
    var buttonText = e.target.innerText;
        if(buttonText == "C"){
         screen = ""
         result.value = screen;
       
    }
    else if(buttonText == "="){
        result.value = eval(screen)
    }else{

        screen += buttonText;
        result.value = screen
    }
  })
}





