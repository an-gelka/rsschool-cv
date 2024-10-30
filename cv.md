# ***ANGELINA POLYAKOVA***
## *FUTURE FRONT-END DEVELOPER*
![avatar](assets/img/2.jpg)
### *Contacts*
* Phone: +375 (29)000-00-00
* E-mail: angelya.050492@gmail.com
* GitHub: an-gelka
* Discord: an-gelka#2009
### *About me*
Recently, I finally decided that it was time to change something in my life and to start changing my field of activity. The idea of going into IT has been haunting me for a long time, I thought for a long time what direction to choose and eventually settled on Frontend development.

I'm new to IT, but I believe that my purposefulness and desire to learn will help me become an experienced Frontend developer in the future.
### *Skills*
* HTML
* CSS
* Java (Fundamentals)
* Git/GitHub
* Editors: Sublime, VSCode
* Figma
### *Code examples*
```
btnElement = document.querySelector(".btn");
resultElement = document.querySelector(".result");
const products = document.querySelectorAll(".item");
inputSurname = document.querySelector('[name="surname"]');
inputName = document.querySelector('[name="name"]');

function totalSumm() {
    sum = 0;
    for (const product of products) {
        let checkboxElement = product.querySelector('input[type="checkbox"]');
        let amountElement = product.querySelector('input[type="number"]');        
            if (checkboxElement.checked) {
                if (amountElement.value <= 0 || amountElement.value > 100) {
                amountElement.value = 1;
                }
            sum += parseInt(checkboxElement.dataset.price) * parseInt(amountElement.value);        
            }        
            else {       
            amountElement.value = 0;        
            }  
        resultElement.textContent = sum; }    
    }    
    btnElement.addEventListener("click" , function(){        
        orderList = [];
        for (const product of products) {
            let choiceElement = product.querySelector('[name="menu"]');
            let amount = product.querySelector('[name="quantity"]');
            if (choiceElement.checked) {
            firstSum = parseInt(choiceElement.dataset.price) * parseInt(amount.value);
            foodName = choiceElement.dataset.goods;
            position = `${foodName} - ${amount.value} шт. = ${firstSum} р.`;
            orderList.push(position);
            }
        }          
        if (orderList == "") {
            alert("Товар не выбран!");
        } else {
            alert (
            `Заказчик: ${inputSurname.value} ${inputName.value}\n\nВаш заказ:\n${orderList.join("\n")}\n\nИтого: ${resultElement.textContent} руб.`
            );
        }
        })
```
### *Education*
* Vitebsk State Technological college
* Belarusian State University (management);
* RS School JavaScript/Front-end (in progress)
### *Language*
* Russian - native
* English - level A2