<html><meta charset='UTF-8'/><meta content='width=device-width, initial-scale=1, user-scalable=1, minimum-scale=1, maximum-scale=5' name='viewport'/><meta content='IE=edge' http-equiv='X-UA-Compatible'/>
<link rel="preconnect" href="https://fonts.googleapis.com"><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin><link href="https://fonts.googleapis.com/css2?family=Ubuntu:wght@400;700&display=swap" rel="stylesheet"><script src="https://cdn.jsdelivr.net/npm/sweetalert2@11.0.19/dist/sweetalert2.all.min.js"></script>
<link href="./style.css" rel="stylesheet" type="text/css" />
<head>
<title>Do You Love Me v2</title>
</head>
<body>
	
   <div id="bodyblur">
    <img src=""/>
   </div>

   <div id='Content'>
   	
     <div id="suratin" onClick="memulai();audio.play();">
       <!-- Surat --><img src="./assets/envelope.png"/>
     </div>
     <p id="ket">Click the Letter!</p>
   
     <div><!-- Foto Akhir Edit di Bagian Bawah--><img src="" id="fotoakhir" /></div>
     <div><blockquote id='bq'>
       <p id="kalimat"></p>
       <p id="kalimatc"></p>
     </blockquote></div>
   
     <!-- Tombol Kirim Pesan -->
     <div id="Tombol">
       <a onClick="sjawab()">
         <b>Send Message</b>
       </a>
     </div>
     
   </div>

<script>function showDiv(){Content.style="opacity:1;margin-top:15vh;",ket.style="margin-top:30px"}function memulai(){suratin.style="transition:all 1s ease;transform:scale(.1);opacity:0",ket.style="transition:all 1s ease;transform:scale(.1);opacity:0",setTimeout(pesan,300)}function kpemb(){suratin.style="display:none",ket.style="display:none",fotoakhir.style="display:inline-flex;transform:scale(1);",Content.style="opacity:1;margin-top:2vh;",bq.style="opacity:1;visibility:visible;margin-top:5px",setTimeout(ngetik,500)}function tombol(){Tombol.style="margin-top:15px;opacity:1;transform: scale(1);",ftom=1}function fakhiran(){document.getElementById("akhiran").style="display:inline-flex"}ftom=0;const swals=Swal.mixin({allowOutsideClick:!1,cancelButtonColor:"#FF0040",imageWidth:100,imageHeight:100}),swalst=Swal.mixin({allowOutsideClick:!1,showConfirmButton:!1,timer:3300,timerProgressBar:!0,imageWidth:100,imageHeight:100}),style=document.createElement("style");var today=new Date,dd=String(today.getDate()).padStart(2,"0"),mm=String(today.getMonth()+1).padStart(2,"0"),yyyy=today.getFullYear();const monthNames=["January","February","March","April","May","June","July","August","September","October","November","December"];function setel(){audio.play()}function setel2(){bgm.play()}function sjawab(){1==ftom&&(Tombol.style="display:none",jawab())}function otomatis(){befanimkata(),setTimeout(animkata,300)}function befanimkata(){kalimatc.style="transform:scale(.3);"}function animkata(){kalimatc.style="transform:scale(1);"}function kemunculan(){otomatis(),kalimatc.innerHTML=ktbwh1,setTimeout(kemunculan2,2200)}function kemunculan2(){otomatis(),kalimatc.innerHTML=ktbwh2,setTimeout(kemunculan3,2200)}function kemunculan3(){otomatis(),kalimatc.innerHTML=ktbwh3,setTimeout(kemunculan,2200)}today=dd+" "+monthNames[today.getMonth()]+" "+yyyy;var katangetik,aa=0;function ngetik(){aa<katangetik.length&&(kalimat.innerHTML+=katangetik.charAt(aa),aa++,setTimeout(ngetik,50)),aa==katangetik.length&&(kalimat.style="margin-bottom:30px","no"==ketrgn?(kalimat.style="margin-bottom:30px",setTimeout(ngetik2,300)):(setTimeout(kemunculan,400),setTimeout(tombol,3e3)))}var katangetik2,ai=0;function ngetik2(){ai<katangetik2.length&&(kalimatc.innerHTML+=katangetik2.charAt(ai),ai++,setTimeout(ngetik2,200)),ai==katangetik2.length&&setTimeout(tombol,500)}</script> <!-- Sampai Sini -->
<script type="text/javascript">
       async function jawab(){await swals.fire('Send me a message on WhatsApp, okay!');window.location = "https://api.whatsapp.com/send?phone=&text=" + pesanwhatsapp;}

      async function pertama(){
         audio = new Audio('');setTimeout(showDiv,100);
       } pertama();
       
      async function pesan(){
                 await swalst.fire({
                  title: 'Hi Cutieee ><', 
                  imageUrl: './assets/cilukba.gif',
                  });   	
                 await swalst.fire({
                  title: 'I Want to Ask You Something 🤭',
                  imageUrl: './assets/gigitin.gif',
                  });
                  var { isConfirmed: prtanya } = await swals.fire({
                        title: `Do You Love Me? 👉🏻👈🏻`,
                        imageUrl: './assets/tarikin.gif',
                        confirmButtonText: 'Love',
                        cancelButtonText: 'No', showCancelButton: true,
                  });
                  if(prtanya){ketrgn = "yes";
                      
                      fotoakhir.src = "./assets/0906-peacegoma.gif";
                      katangetik = "Yayyy! If you love me, I just want to tell you...         ";
                      ktbwh1 = "I LOVE YOU❤️";
                      ktbwh2 = "Never Leave Me🥺";
                      ktbwh3 = "Always Stay With Me🤭";
                      pesanwhatsapp = "I love you. I Love You too ><";
                      
                  } else {ketrgn = "no";
                      
                      fotoakhir.src = "./assets/wortel.gif";
                      katangetik = "Aww🥺 okay then if you don't love me :(         ";
                      katangetik2 = "See Youuu";
                      pesanwhatsapp = "I don't love you :(";
                  }
                 
                  setTimeout(kpemb,300);
       }
</script>
</body>
</html>
