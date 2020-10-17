//bài 1-DOM
    // var inputName1=prompt("Mời bạn nhập tên:");
    // var inputOld1=prompt("Mời bạn nhập tuổi:");
    // var button1=document.querySelector("div#bai1 button.btn-bai1");
    // button1.addEventListener("click",function(){
    //     document.writeln("Tên của bạn là: ",inputName1.value);
    //     document.writeln("Tuổi của bạn là:",inputOld1.value);
    // })
//bài 2-DOM
var inputNameEx2=document.querySelector("div#bai2 input.inputName2");
var button2=document.querySelector("div#bai2 button.btn-bai2");
// console.log(inputNameEx2,button2);
button2.addEventListener("click",function(){
    alert("Xin chào: "+inputNameEx2.value);
})

//bài 3-DOM
var inputNameEx3=document.querySelector("div#bai3 input.inputName3");
var resultEx3=document.querySelector("div#bai3 input.result");
var button3=document.querySelector("div#bai3 button.btn-bai3");
button3.addEventListener("click",function(){
    return resultEx3.value="xin chào: "+inputNameEx3.value;
})

//bài 4-DOM
var inputYear=document.querySelector("div#bai4 input.year");
var outputOld=document.querySelector("div#bai4 input.old");
var outputResult=document.querySelector("div#bai4 button.resultEx4");
// console.log(inputYear,outputResult,outputOld);
outputResult.addEventListener("click",function(){
    return outputOld.value=2020-inputYear.value;
})

//bài 6-DOM
var mauxanh=document.querySelector("div#bai6 button.blue");
var maudo =document.querySelector("div#bai6 button.red");
var divEx6=document.getElementById("bai6");
mauxanh.addEventListener("click", function(){
    divEx6.style.backgroundColor="blue";
})
maudo.addEventListener("click",function(){
    divEx6.style.backgroundColor="red";
})
//bài 7-DOM
var button7=document.querySelector("div#bai7 button.btn-bai7");
var selector7=document.querySelector("div#bai7 select.selector");
var divEx7=document.getElementById("bai7");
button7.addEventListener("click",function(){
    return Chonmau();
})
function chonmau(){
    var operator=selector7.value;
    var divbai7=divEx7.value;
    switch(operator){
        case"do":
            divbai7.style.backgroundColor="red";
            break;
        case"xanhduong":
            divbai7.style.backgroundColor="blue";
            break;
        case"xanhla":
            divbai7.style.backgroundColor="green";
            break;
        case"vang":
            divbai7.style.backgroundColor="yellow";
            break;
    }
    return divbai7;
}
//Bài 12-DOM
var soluong=document.querySelector("div#bai12 input.inputsoluong");
var dongia=document.querySelector("div#bai12 input.inputdongia");
var thanhtien=document.querySelector("div#bai12 input.outputthanhtien");
var button12=document.querySelector("div#bai12 button.tinh");
// console.log(soluong,dongia,thanhtien,button12);
button12.addEventListener("click",function(){
    return thanhtien.value=soluong.value*dongia.value;
})
// Bài 13-DOM
var start=document.querySelector("div#bai13 button.btn-start");
var stopp=document.querySelector("div#bai13 button.btn-stop");
var reset=document.querySelector("div#bai13 button.btn-reset");
var h3=document.getElementById("display");
var giay=0,phut=0,gio=0,t,tichtac=0;
start.addEventListener("click",function(){
    return run();
})
function add(){
    tichtac++;
    if(tichtac==300){
        giay++;
        tichtac=0;
        if(giay==60){
            giay=0;
            phut++;
            if(phut==60){
                phut=0;
                gio++;
                if(gio==24){
                    gio=0;
                }
            }
        }
    }
    h3.textContent= (gio ? (gio > 9 ? gio : "0" + gio) : "00") + ":" + (phut ? (phut > 9 ? phut : "0" + phut) : "00") + ":" + (giay > 9 ? giay : "0" + giay)+ ":" + (tichtac > 9 ? tichtac : "00" + tichtac ||tichtac>99 ? tichtac:"0");
}
function run(){
    t = setInterval(add,1);
}
stopp.addEventListener("click",function (){
    clearInterval(t);
})
reset.onclick = function (){
    h3.textContent="00:00:00";
    giay=0,phut=0,gio=0;
}
//Bài 5_DOM
var namsinh=document.querySelector("div#bai5 input.date");
var button5=document.querySelector("div#bai5 button.btn-bai5");
button5.addEventListener("click",function(){
    if(namsinh.value>2020){
        alert("Nhập lại");
    }
    else{
        alert("đã kiểm tra");
    }
})
