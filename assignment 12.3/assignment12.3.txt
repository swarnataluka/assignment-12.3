Object.map=function(array1,number1){ 
    var result=[];
    Object.keys(array1).forEach(function(number2){ 
        result[number2]=number1.call(array1,array1[number2]);
    });
        return result; 
    }

    mapResult=Object.map([2,4,6],function(num){ 
        return num * 2;
    });