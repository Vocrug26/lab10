# lab10
<h1 align="center">МИНИСТЕРСТВО НАУКИ И ВЫСШЕГО ОБРАЗОВАНИЯ РОССИЙСКОЙ ФЕДЕРАЦИИ ФЕДЕРАЛЬНОЕ ГОСУДАРСТВЕННОЕ БЮДЖЕТНОЕ ОБРАЗОВАТЕЛЬНОЕ УЧРЕЖДЕНИЕ ВЫСШЕГО ОБРАЗОВАНИЯ «САХАЛИНСКИЙ ГОСУДАРСТВЕННЫЙ УНИВЕРСИТЕТ»</h1>
<p align="center">Лабораторная работа №6</p>
<p align="center">Лабораторная работа №8</p>
<p align="center">"JavaScript"</p>
<br>
<p align="right">Работу выполнил Гурков Владислав Викторович</p>
<p align="right">Работу проверил Соболев Евгений Игоревич</p>
### **Цели и задачи:**
1.	Напишите функцию, которая найдёт числа в массиве, которые делятся на заданное число. 
2.	Нужно написать функцию, которая проверяет, являются ли две строки анаграммами, причем регистр букв не имеет значения. Учитываются лишь символы; пробелы или знаки препинания в расчет не берутся.
3.	Нужно написать функцию, принимающую строку в качестве аргумента и возвращающую количество гласных, которые содержатся в строке.
Гласными являются «a», «e», «i», «o», «u».
4.	Треугольник. Напишите цикл,  выводит такой треугольник:
1
2
3
4
5
6
7	#
##
###
####
#####
######
#######
5.	FizzBuzz. Напишите программу, которая выводит через console.log все числа от 1 до 100, с двумя исключениями. Для чисел, нацело делящихся на 3, она должна выводить ‘Fizz’, а для чисел, делящихся на 5 (но не на 3) – ‘Buzz’.Когда сумеете – исправьте её так, чтобы она выводила «FizzBuzz» для всех чисел, которые делятся и на 3 и на 5.
6.	Шахматная доска. Напишите программу, создающую строку, содержащую решётку 8х8, в которой линии разделяются символами новой строки. На каждой позиции либо пробел, либо #. 
7.	Минимум. Напишите функцию min, принимающую два аргумента, и возвращающую минимальный из них.
8.	Рекурсия. Ноль чётный. Единица нечётная. У любого числа N чётность такая же, как у N-2. Напишите рекурсивную функцию isEven согласно этим правилам. Она должна принимать число и возвращать булевское значение. Потестируйте её на 50 и 75. Попробуйте задать ей -1. Почему она ведёт себя таким образом? Можно ли её как-то исправить?
9.	Считаем бобы. Символ номер N строки можно получить, добавив к ней .charAt(N) ( “строчка”.charAt(5) ) – схожим образом с получением длины строки при помощи .length. Возвращаемое значение будет строковым, состоящим из одного символа (к примеру, “к”). У первого символа строки позиция 0, что означает, что у последнего символа позиция будет string.length – 1. Другими словами, у строки из двух символов длина 2, а позиции её символов будут 0 и 1.Напишите функцию countBs, которая принимает строку в качестве аргумента, и возвращает количество символов “B”, содержащихся в строке.Затем напишите функцию countChar, которая работает примерно как countBs, только принимает второй параметр — символ, который мы будем искать в строке (вместо того, чтобы просто считать количество символов “B”). Для этого переделайте функцию countBs.
10.	Сумма диапазона.  Напишите функцию range, принимающую два аргумента, начало и конец диапазона, и возвращающую массив, который содержит все числа из него, включая начальное и конечное.Затем напишите функцию sum, принимающую массив чисел и возвращающую их сумму. Запустите указанную выше инструкцию и убедитесь, что она возвращает 55.В качестве бонуса дополните функцию range, чтобы она могла принимать необязательный третий аргумент – шаг для построения массива. Если он не задан, шаг равен единице. Вызов функции range(1, 10, 2) должен будет вернуть [1, 3, 5, 7, 9]. Убедитесь, что она работает с отрицательным шагом так, что вызов range(5, 2, -1) возвращает [5, 4, 3, 2].
11.	Обращаем массив вспять. Напишите две функции, reverseArray и reverseArrayInPlace. Первая получает массив как аргумент и выдаёт новый массив, с обратным порядком элементов. Вторая работает как оригинальный метод reverse – она меняет порядок элементов на обратный в том массиве, который был ей передан в качестве аргумента. Не используйте стандартный метод reverse.
12.	Глубокое сравнение. Оператор == сравнивает переменные объектов, проверяя, ссылаются ли они на один объект. Но иногда полезно было бы сравнить объекты по содержимому. Напишите функцию deepEqual, которая принимает два значения и возвращает true, только если это два одинаковых значения или это объекты, свойства которых имеют одинаковые значения, если их сравнивать рекурсивным вызовом deepEqual. Чтобы узнать, когда сравнивать величины через ===, а когда – объекты по содержимому, используйте оператор typeof. Если он выдаёт “object” для обеих величин, значит нужно делать глубокое сравнение. Не забудьте об одном дурацком исключении, случившемся из-за исторических причин: “typeof null” тоже возвращает “object”.
13.	Свертка. Используйте метод reduce в комбинации с concat для свёртки массива массивов в один массив, у которого есть все элементы входных массивов.

```
 function z1()
        {
            let mass = [1, 2, 3, 4, 5, 6, 7, 8, 9];
            let n =3;
            let vivod=""; 
            for (let i = 0; i < mass.length; i++)
            {
                if (mass[i]%n==0)
                {
                    vivod += mass[i]+ ", ";
                }
            }
            console.log(vivod);
        }

        function z2()
        {
            let str1 = "Banana milk";
            let str2 = "Banana milk";
            annagram(str1, str2);
        }

        function annagram(str1, str2)
        {
            let result = false;
            document.getElementById("aa").innerHTML =str1 + ".   " +str2;
            let arr1 = [];
            let arr2 = [];
            for (let i = 0; i < str1.length; i++)
            {
                if ((str1[i] != ' ')&&(str1[i] != ',')&&(str1[i] != '!')&&(str1[i] != '?')&&(str1[i] != '.'))
                {arr1.push(str1[i]);}
            }
            for (let i = 0; i < str2.length; i++)
            {
                if ((str2[i] != ' ')&&(str2[i] != ',')&&(str2[i] != '!')&&(str2[i] != '?')&&(str2[i] != '.'))
                {arr2.push(str2[i]);}
            }
            if (arr1.length != arr2.length)
            {
                result = false;
            }
            else
            {
                result = true;
                for (let i = 0; i < arr1.length; i++)
                {
                    if (arr1[i] != arr2[i])
                    {
                        result = false;
                    }
                }
            }
            document.getElementById("aa").innerHTML +=" результат: " + result;
        }

        function words()
        {
            var count=0; 
            var str1 = "Banana milk";
            var gl = ["a","e","i","o","u"];
            for (let char of str1)
            {
                if(gl.includes(char))
                {count++;}
            }
            document.getElementById("bb").innerHTML =" Количество гласных равно: " + count;
        }

        function stairs()
        {   
            let les="#";
            let str = "";
            for (let i=0; i < 7; i++)
            {   
                str += les;
                console.log(str);

            }
        }

        function FizzBuzz()
        {
            let str=0;
            for (let i = 1; i <= 100 ; i++)
            {
                str = i;
                if (i%3==0)
                {
                    str = "Fizz";
                }
                if (i%5==0)
                {
                    str = "Buzz";
                }
                if ((i%5==0)&&(i%3==0))
                {
                    str = "FizzBuzz";
                }
                console.log(str);
            }
        }

        function Chess()
        {
            for (q = 1; q <= 4; q ++) 
            {
                var l = "#";
                for (var cont = 1; cont < 4; cont ++)
                    l += '  #';
                console.log(l);
                var m ='';
                for (var cont = 0; cont < 4; cont ++)
                m += '  #';
                console.log(m);
            }
        }

        function min(a,b)
        {
            a = 10;
            b = 9;
            if (a>b)
            {
                document.getElementById("cc").innerHTML ="Minimum: " + b; 
            }
            else 
            {
                document.getElementById("cc").innerHTML ="Minimum: " + a;
            }
        }
        function isEven(N)
        {   
            if (Math.abs(N)==0)
                {return 'true';}
            else if (Math.abs(N)==1)
                {return 'false';}
            else 
                {return isEven(N-2)};
        }
        function z8()
        {
            console.log(isEven(50));
            console.log(isEven(75));
            console.log(isEven(-1));
        }
        
        function countBs(str)
        {
            let count = 0;
            for (let i=0; i < str.length ; i++)
            {
                if (str[i]=="B")
                count +=1;
            }
            return count;
        }

        function countChar(str,ch)
        {
            let count = 0;
            for (let i=0; i < str.length ; i++)
            {
                if (str[i]==ch)
                count +=1
            }
            return count;
        }
        function z9()
        {   
            let str = "Bob eats carrot"
            let ch = "r"
            console.log(countBs(str));
            console.log(countChar(str,ch));
        }


        function range(b,e,step)
        {   
            if (step==null)
            step = 1;
            var mass = [];
            if (step > 0)
            {
                for (var i=b ;i <= e ; i +=step)
                {
                    mass.push(i);
                } 
            }
            else 
            {
                for (var i=b ;i >= e ; i +=step)
                {
                    mass.push(i);
                } 
            }
           return mass;
        }

        function sum(mass)
        {
            let summa=0;
            for (var i = 0; i < mass.length ; i++)
            {
                summa += mass[i];
            }
           return summa;  
        }

        function z10()
        {
            console.log(range(1,10));
            console.log(sum(range(1,10)));
            console.log(sum(range(5, 2, -1)));
        }
        function reverseArray(arr)
        {
            let i;
            let result = [];
            for (i=arr.length-1;i>=0;i--)
            {
                result.push(arr[i]);
            }
            return result;
        }
        
        function reverseArrayInPlace(arr) 
        {
            let i,old;
            for ( i = 0; i < Math.floor(arr.length / 2); i++ ) 
            {
                old = arr[i];
                arr[i] = arr[arr.length - (1 + i)];
                arr[arr.length - (1 + i)] = old;
            }
            return arr;
        }

        function z11()
        {
            console.log(reverseArray([1,2,3,4,5]));
            console.log(reverseArrayInPlace([1,2,3,4,5]));
        }
        
        function deepEqual(a, b)
        {
        if (a === b) {
            return true;
        }
 
            if (a == null || typeof(a) != "object" ||
            b == null || typeof(b) != "object")
            {
                return false;
            }
 
        var propertiesInA = 0, propertiesInB = 0;
        for (var property in a) {
            propertiesInA += 1;
        }
        for (var property in b) {
            propertiesInB += 1;
            if (!(property in a) || !deepEqual(a[property], b[property])) {
            return false;        
            }
        }        
        return propertiesInA == propertiesInB;
        }
        function z12()
        {
            var obj = {here: {is: "an"}, object: 2};
            console.log(deepEqual(obj, obj));        
            console.log(deepEqual(obj, {here: 1, object: 2}));
            console.log(deepEqual(obj, {here: {is: "an"}, object: 2}));
        }

        function z13()
        {
            const numbers = [1,2,3,4];
            const numbers2 = [5,6,7,8];
            const num = numbers.concat(numbers2);
            let sum = num.reduce(myFunction);
            document.getElementById("demo").innerHTML = "Otvet: " + sum;
        }

        function myFunction(total, value) 
        {
            return total + value;
        }
```
### **Вывод:**
После выполнения данной лабораторной работы я улучшил свои навыки работы с JavaScript.
