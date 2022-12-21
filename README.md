# agar.io-mods
This is a javascript movement mod that allows you to use arrow keys instead of mouse for movement (Bookmarklet)
MAKE SURE TO ONLY TURN ON IF YOU ARE ALREADY LOADED INTO THE ROUND, OTHERWISE IT WON'T WORK
javascript:a=document.getElementById("canvas"),b=this.onkeydown,c=this.onkeyup,d=a.onmousemove,e=a.width/2,f=a.height/2,this.onkeydown=function(g){b(g),37!=g.keyCode||(e=-100000),40!=g.keyCode||(f=100000),38!=g.keyCode||(f=-100000),39!=g.keyCode||(e=100000),d({clientX:e,clientY:f})},this.onkeyup=function(g){c(g),37!=g.keyCode||(e=a.width/2),40!=g.keyCode||(f=a.height/2),38!=g.keyCode||(f=a.height/2),39!=g.keyCode||(e=a.width/2),d({clientX:e,clientY:f})},a.onmousemove=null,alert("You're ready to play Agar.io with arrow keys, by LogikKidGuy!");
