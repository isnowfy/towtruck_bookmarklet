[towtruck](https://github.com/mozilla/towtruck) bookmarklet

~~~~
javascript:(function(){if(typeof tow_bm_loaded!='undefined' && tow_bm_loaded){tow_bm_loaded=false;var s=document.getElementById('tow_bm_s');s.remove();var d=document.getElementById('tow_bm_d');d.remove();}else{var s=document.createElement('script');s.src='https://towtruck.mozillalabs.com/towtruck.js';s.id='tow_bm_s';s.onload=function(){tow_bm_loaded=true;var d=document.createElement('div');d.innerHTML='<button onclick=%22TowTruck(this); return false;%22 style=%22position:fixed;left:10px;bottom:0;border:1px solid #FFF;background:#05A44F;%22>Start TowTruck</button>';d.id='tow_bm_d';document.body.appendChild(d);};document.head.appendChild(s);}})();
~~~~

you can put the code above to your bookmark to use towtruck
