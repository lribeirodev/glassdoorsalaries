# glassdoorsalaries
##### scrolldown for english version 

# VERSÃO PORTUGUÊS
##### Este código converte e mostra o salário de USD para BRL
acesse o site www.glassdoor.com <br>
procure por salários nos estados unidos <br>

# Método um <br>

abra devtools no seu navegador <br>
copie e cole o código abaixo <br>
```
data = document.getElementsByClassName('m-0 css-g261rn');
dinheiros = prompt('Valor Dolar Hoje? exemplo 5.40 ou 5,40');
dinheiros = dinheiros.replaceAll(',','.');
salarys = [];
salarysPerMonth = [];
[].forEach.call(data,function(x,i){salary = x.textContent; if(salary.includes('US$')) salarys.push(salary);});
salarys.forEach(function(data){d = data.replaceAll('US$',""); d = eval(d) / 12; salarysPerMonth.push(d);});
salarysPerMonth.forEach(function(data,i){this[i] = (this[i] * 1000).toLocaleString('en-Us',{style:'currency', currency: 'USD',})},salarysPerMonth);
salarys.forEach(function(x,j){for(let i = 0; i < data.length ; i++){if(data[i].textContent.includes(x) && !data[i].textContent.includes('[') && data[i].textContent.length > 6){data[i].textContent = data[i].textContent + ' [ US' + salarysPerMonth[j] + ' ' + new Intl.NumberFormat('pt-BR', { style: 'currency', currency: 'BRL' }).format(eval(salarysPerMonth[j].replace(/([\,\$])+/g,'').replaceAll(',','.')) * dinheiros) + ' ]'; break;} }},salarys);
```
aperte o enter do teclado<br>
uma janela vai aparecer e solicitar o valor da cotação do dolar atual<br>
aperte enter novamente<br>
aproveite<br>

# Método dois <br>
aperte ctrl+d no teclado<br>
clique no botão mais<br>
mude a url do favorito para o código abaixo<br>
```
javascript:(function(){data = document.getElementsByClassName('m-0 css-g261rn'); dinheiros = prompt('Valor Dolar Hoje? exemplo 5.40 ou 5,40'); dinheiros = dinheiros.replaceAll(',','.'); salarys = []; salarysPerMonth = []; [].forEach.call(data,function(x,i){salary = x.textContent; if(salary.includes('US$')) salarys.push(salary);}); salarys.forEach(function(data){d = data.replaceAll('US$',""); d = eval(d) / 12; salarysPerMonth.push(d);}); salarysPerMonth.forEach(function(data,i){this[i] = (this[i] * 1000).toLocaleString('en-Us',{style:'currency', currency: 'USD',})},salarysPerMonth); salarys.forEach(function(x,j){for(let i = 0; i < data.length ; i++){if(data[i].textContent.includes(x) && !data[i].textContent.includes('[') && data[i].textContent.length > 6){data[i].textContent = data[i].textContent + ' [ US' + salarysPerMonth[j] + ' ' + new Intl.NumberFormat('pt-BR', { style: 'currency', currency: 'BRL' }).format(eval(salarysPerMonth[j].replace(/([\,\$])+/g,'').replaceAll(',','.')) * dinheiros) + ' ]'; break;} }},salarys);})()
```
mude o nome do favorito conforme a sua vontade<br>
clique no favorito que você salvou<br>
aperte o enter do teclado<br>
uma janela vai aparecer e solicitar o valor da cotação do dolar atual<br>
aperte enter novamente<br>
agora você pode utilizar o código quando quiser<br>
aproveite<br>


# ENGLISH VERSION 
##### this code convert and show the salary from usa to brl
open the www.glassdoor.com <br>
search for salaries in USA <br>

# Method One <br>
open devtools from your browser <br>
copy paste the code below <br>
```
data = document.getElementsByClassName('m-0 css-g261rn');
dinheiros = prompt('Valor Dolar Hoje? exemplo 5.40 ou 5,40');
dinheiros = dinheiros.replaceAll(',','.');
salarys = [];
salarysPerMonth = [];
[].forEach.call(data,function(x,i){salary = x.textContent; if(salary.includes('US$')) salarys.push(salary);});
salarys.forEach(function(data){d = data.replaceAll('US$',""); d = eval(d) / 12; salarysPerMonth.push(d);});
salarysPerMonth.forEach(function(data,i){this[i] = (this[i] * 1000).toLocaleString('en-Us',{style:'currency', currency: 'USD',})},salarysPerMonth);
salarys.forEach(function(x,j){for(let i = 0; i < data.length ; i++){if(data[i].textContent.includes(x) && !data[i].textContent.includes('[') && data[i].textContent.length > 6){data[i].textContent = data[i].textContent + ' [ US' + salarysPerMonth[j] + ' ' + new Intl.NumberFormat('pt-BR', { style: 'currency', currency: 'BRL' }).format(eval(salarysPerMonth[j].replace(/([\,\$])+/g,'').replaceAll(',','.')) * dinheiros) + ' ]'; break;} }},salarys);
```
hit enter button<br>
the prompt will be showed, you have to put the cotation from usd today<br>
hit enter again<br>
enjoy<br>

# Method Two <br>
hit ctrl+d<br>
click more button<br>
change the url link from the code above<br>
```
javascript:(function(){data = document.getElementsByClassName('m-0 css-g261rn'); dinheiros = prompt('Valor Dolar Hoje? exemplo 5.40 ou 5,40'); dinheiros = dinheiros.replaceAll(',','.'); salarys = []; salarysPerMonth = []; [].forEach.call(data,function(x,i){salary = x.textContent; if(salary.includes('US$')) salarys.push(salary);}); salarys.forEach(function(data){d = data.replaceAll('US$',""); d = eval(d) / 12; salarysPerMonth.push(d);}); salarysPerMonth.forEach(function(data,i){this[i] = (this[i] * 1000).toLocaleString('en-Us',{style:'currency', currency: 'USD',})},salarysPerMonth); salarys.forEach(function(x,j){for(let i = 0; i < data.length ; i++){if(data[i].textContent.includes(x) && !data[i].textContent.includes('[') && data[i].textContent.length > 6){data[i].textContent = data[i].textContent + ' [ US' + salarysPerMonth[j] + ' ' + new Intl.NumberFormat('pt-BR', { style: 'currency', currency: 'BRL' }).format(eval(salarysPerMonth[j].replace(/([\,\$])+/g,'').replaceAll(',','.')) * dinheiros) + ' ]'; break;} }},salarys);})()
```
change the favorite name as you want<br>
click on the favorite that you saved it<br>
the prompt will be showed, you have to put the cotation from usd today<br>
hit enter again<br>
now you can use the code whenever you want<br>
enjoy

