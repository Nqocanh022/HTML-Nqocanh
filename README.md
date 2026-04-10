<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <script>
        // KIỂM TRA CHẴN LẺ 
        let n =prompt("Nhập số: ");
        if(n%2==0){
            console.log('Số chẵn');
        }
        else{
            console.log('Số lẻ');
        }


        //Kiểm tra số nguyên tố 
let m = prompt("Nhập dữ liệu");
let songuyento = function(m){
    m = Number(m);
    if(m < 2){ 
        console.log("false");
        return;
    }
    for(let i = 2; i <= Math.sqrt(m); i++){
        if(m % i == 0){ 
            console.log("false");
            return; 
        }
    }
    console.log("true");
}
songuyento(m);
 // số nguyên tố từ 1-n 
 let h =prompt("Nhập giá trị của h: ");
 let list =function(h){
    h = Number(h);
    for(let i=1;i<=h;i++){
        let check=true;
        if(i<2) continue;
        for(let j=2;j<=Math.sqrt(i);j++){
            if(i%j==0){
                check=false;
                break;
            }
        }
        if(check) console.log(i);
    }
 }
 list(h);
 let c=Number(prompt("tính tổng số"));
 let sum=0;
    for(let i=1;i<=c;i++){
        if(i%3==0||i%5==0){
            sum+=i;
        }
    }   
    console.log(sum);
    </script>
</html>
