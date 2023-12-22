<h1 align= "center"> МИНИСТЕРСТВО НАУКИ И ВЫСШЕГО ОБРАЗОВАНИЯ РОССИЙСКОЙ ФЕДЕРАЦИИ ФЕДЕРАЛЬНОЕ ГОСУДАРСТВЕННОЕ БЮДЖЕТНОЕ ОБРАЗОВАТЕЛЬНОЕ УЧРЕЖДЕНИЕ ВЫСШЕГО ОБРАЗОВАНИЯ «САХАЛИНСКИЙ ГОСУДАРСТВЕННЫЙ УНИВЕРСИТЕТ»</h1>
<br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>
<p align= "center">Лабораторная работа №6</p><br><br><br><br><br><br><br><br>
<p align= "right">Выполнил: Акимов И.В.</p><br><br><br><br><br><br><br><br>
<p align="center">г. Южно-Сахалинск <br> 2023 год</p><br><br><br><br><br><br><br><br>
<h2 style="text-align: center">Введение</h2>
<p align="justify">JavaScript ("JS" для краткости) — это полноценный динамический язык программирования, который применяется к HTML документу, и может обеспечить динамическую интерактивность на веб-сайтах. Его разработал Brendan Eich, сооснователь проекта Mozilla, Mozilla Foundation и Mozilla Corporation. JavaScript сам по себе довольно компактный, но очень гибкий. Разработчиками написано большое количество инструментов поверх основного языка JavaScript, которые разблокируют огромное количество дополнительных функций с очень небольшим усилием. JavaScript невероятно универсален и дружелюбен к новичкам. Обладая большим опытом, вы сможете создавать игры, анимированную 2D и 3D графику, полномасштабные приложения с базами данных и многое другое!</p>
<h2 style="text-align: center">Цели и задачи</h2>
<ol align="justify"> <br>
1.	Сделайте alert по нажатию на кнопку.

            <p>
              <button onclick="func1()">1 Задание</button>
          </p>
          function func1() {
              alert("Кнопка была нажата!");
            }
            
2.	Сделайте изменение текста в input по нажатию кнопки.

          <p>
              <button onclick="func2()">2 Задание</button>
              <input type="text" id="myInput" value="kanon">
          </p>
           function func2() {
              var input = document.getElementById('myInput');
              input.value = "Новый текст!";
            }
 
3.	Сделайте вывод содержимого input по нажатию кнопки.

       <p>
              <button onclick="func3()">3 Задание</button>
              <input type="text" id="myInput" value="like">
      </p>
        function func3() {
              var input = document.getElementById('myInput').value;
              alert(input);
            }
  
  4.	 Сделайте кнопку по нажатию на нее, она выводит alert содержимое input, возведенное в квадрат.

                <p>
                  <button onclick="func4()">4 Задание</button>
                  <input type="num" id="myInput" value="5">
                </p>
                  	 function func4() {
                  alert(Math.pow(document.getElementById('myInput').value, 2))
                }
                  
  5.	 Сделайте кнопку по нажатию, она осуществляет обмен содержимым между двумя input.

               <p>
                  <button onclick="func5()">5 Задание</button>
                  <input type="text" id="input31" value="like">
                  <input type="text" id="input32" value="boss">
                </p>
                function func5() {
                    var temp = document.getElementById('input31').value; 
                    document.getElementById('input31').value = document.getElementById('input32').value; 
                    document.getElementById('input32').value = temp;
                  }
  
  6.	Сделайте кнопку по нажатию на нее поменяется ее текст.

              <p>
                <button onclick="this.innerHTML = 'Текст поменялся'">6 Задание</button>
              </p>
              	function func6() {
              this.innerHTML = 'Текст кнопки поменялся';
            }
  
  7.	Сделайте кнопку по нажатию на нее, она меняет цвет текста в input, используя свойства CSS.

                <p>
                  <button onclick="func7()">7 Задание</button>
                  <input type="text" id="Inputs" value="asdadszbnm">
                </p>
                function func7() {
              document.getElementById('Inputs').style.color = 'blue'
            }
  
  8.	Сделайте кнопки по нажатию на них, одна из них блокирует input с помощью атрибута disabled, а другая разблокирует.

          <p>
          <button onclick="func8()">8 Задание</button>
          <button onclick="func88()">8 Задание</button>
          <input type="text" id="Innput" value="awsdzxcfvg">
        </p>

        function func8() {
            document.getElementById('Innput').disabled = true;
              }
              function func88() {
                document.getElementById('Innput').disabled = false;
                  }
  
  9.	Сделайте кнопку при наведении на нее появляется alert.
        
        <p>
          <button onmouseover="alert('Вы навелись на кнопку')">9 Задание</button>
        </p>

  
  10.	 Сделайте кнопку при двойном на нее появляется alert.

          <p>
            <button ondblclick="alert('двойное нажатие')">10 Задание</button>
          </p>
            <style>
              .a {
               border: 2px double rgb(233, 4, 4); 
               background-color: rgb(6, 3, 167);
               width:130px;
              }
             </style>
            
  
  11.	 Сделайте область с помощью div при наведении на нее появляется alert.
            
            <p>
              <div class="a" onmouseover="alert('Наведение ')">11 ЗАДАНИЕ</div>
            
            </p>

  12.	Сделайте кнопку и картинку, при нажатии кнопки картинка меняется.

          <p>
            <button onclick="func12()">12 Задание</button><br>
            <img id="myImage" src="anima.jpeg" width="200" height="200">
          </p>
             function func12() {
             document.getElementById('myImage').src = 'anim.jpg'
            }

  13.	Сделайте alert по нажатию на кнопку. Используя this.

            <p>
              <button onclick="alert(this.innerHTML)">13 Задание</button>
            </p>

  14.	Сделайте изменение текста в input по нажатию кнопки. Используя this.

            <p>
              <input type="text" id="Inputqq" value="sdadadsajklghy">
              <button onclick="this.previousElementSibling.value = 'Изменён'">14 Задание</button>
            </p>

  15.	Сделайте кнопку, при нажатии кнопки кнопка блокируется.
            
            <p>
              <button onclick="this.disabled = true;">15 Задание</button>
            </p>

  16.	Сделайте кнопку, при нажатии кнопка считает количество нажатий на нее.

             < p>
                <button onclick="func16()">16 Задание</button>
              <p id="clickCount">Количество нажатий: 0</p>
              </p>
              var clickCount = 0;
              function func16() {
                clickCount++;
                document.getElementById("clickCount").innerHTML = "Количество нажатий: " + clickCount;
                }

  17.	Сделайте кнопку, при нажатии курсор мышки должен измениться.
            
            <p>
              <button onclick="this.style.cursor = 'pointer'">17 Задание</button>
            </p>

  18.	Используя JavaScript, сделайте так, чтобы при клике на кнопку исчезал элемент с id=&quot;hide&quot
            <!DOCTYPE HTML>
            <html>
            <head>
                <meta charset="utf-8">
            </head>
            <body>
                <input type="button" id="hider" value="Нажмите, чтобы спрятать текст"/>
                <div id="hide">Текст</div>
            <script>
                /* ваш код */
            </script>
            </body>
            </html>
            <p>
              <button onclick="func18()">18 Задание</button>
              <p id="hide">id=hide</p>
            </p>
             	function func18() {
              document.getElementById('hide').style.display = 'none';
          }


19.	Создайте кнопку, при клике на которую, она будет скрывать сама себя.

        function func19() {
          const massive = [10, 5, 20, 8, 15, 30, 25, 12];  
          let minel = massive[0];
          let maxel = massive[0];
          let indexmin = 0;
          let indexmax = 0;
          for (let i = 1; i < massive.length; i++) {
            if (massive[i] < minel) {
              minel = massive[i];
              indexmin = i;
            }
            if (massive[i] > maxel) {
              maxel = massive[i];
              indexmax = i;
            }
          }
           	const sumindex = indexmin + indexmax;
          alert('Сумма номеров минимального и максимального элементов: ' + sumindex);
          }
       < p>
          <button onclick="this.style.display = 'none'">19 Задание</button>
        </p>
  

20.	Напишите простой калькулятор.

          function func20() {
            function calculate(num1, operator, num2) {
              switch (operator) {
                case '+':
                  return num1 + num2;
                case '-':
                  return num1 - num2;
                case '*':
                  return num1 * num2;
                case '/':
                  if (num2 !== 0) {
                    return num1 / num2;
                  } else {
                    return 'Ошибка: Деление на ноль невозможно!';
                  }
                default:
                  return 'Ошибка: Неверный оператор!';
              }
            }
            const number1 = parseFloat(prompt('Введите первое число:'));
            const operator = prompt('Введите оператор (+, -, *, /):');
            const number2 = parseFloat(prompt('Введите второе число:'));
            const result = calculate(number1, operator, number2);
            alert(`Результат: ${result}`);
          }
  <p>
  <button onclick="func20()">20 Задание</button>
</p>
### вывод
Написал простой сайт о себе c блоками, header, nav, footer, используете три движка pug, handlebars, EJS
