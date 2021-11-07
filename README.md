# glassdoorsalaries
this code convert and show the salary from usa to brl


open the www.glassdoor.com
search for salaries in USA
open devtools from your browser

[Method one]
copy paste the code below

data = document.getElementsByClassName('m-0 css-g261rn');
dinheiros = prompt('Valor Dolar Hoje? exemplo 5.40 ou 5,40');
dinheiros = dinheiros.replaceAll(',','.');
salarys = [];
salarysPerMonth = [];
[].forEach.call(data,function(x,i){salary = x.textContent; if(salary.includes('US$')) salarys.push(salary);});
salarys.forEach(function(data){d = data.replaceAll('US$',""); d = eval(d) / 12; salarysPerMonth.push(d);});
salarysPerMonth.forEach(function(data,i){this[i] = (this[i] * 1000).toLocaleString('en-Us',{style:'currency', currency: 'USD',})},salarysPerMonth);
salarys.forEach(function(x,j){for(let i = 0; i < data.length ; i++){if(data[i].textContent.includes(x) && !data[i].textContent.includes('[') && data[i].textContent.length > 6){data[i].textContent = data[i].textContent + ' [ US' + salarysPerMonth[j] + ' ' + new Intl.NumberFormat('pt-BR', { style: 'currency', currency: 'BRL' }).format(eval(salarysPerMonth[j].replace(/([\,\$])+/g,'').replaceAll(',','.')) * dinheiros) + ' ]'; break;} }},salarys);
hit enter button
the prompt will be showed, you have to put the cotation from usd today
hit enter again
enjoy

[method two]
hit ctrl+d
click more button
change the url link from the code above
javascript:(function(){data = document.getElementsByClassName('m-0 css-g261rn'); dinheiros = prompt('Valor Dolar Hoje? exemplo 5.40 ou 5,40'); dinheiros = dinheiros.replaceAll(',','.'); salarys = []; salarysPerMonth = []; [].forEach.call(data,function(x,i){salary = x.textContent; if(salary.includes('US$')) salarys.push(salary);}); salarys.forEach(function(data){d = data.replaceAll('US$',""); d = eval(d) / 12; salarysPerMonth.push(d);}); salarysPerMonth.forEach(function(data,i){this[i] = (this[i] * 1000).toLocaleString('en-Us',{style:'currency', currency: 'USD',})},salarysPerMonth); salarys.forEach(function(x,j){for(let i = 0; i < data.length ; i++){if(data[i].textContent.includes(x) && !data[i].textContent.includes('[') && data[i].textContent.length > 6){data[i].textContent = data[i].textContent + ' [ US' + salarysPerMonth[j] + ' ' + new Intl.NumberFormat('pt-BR', { style: 'currency', currency: 'BRL' }).format(eval(salarysPerMonth[j].replace(/([\,\$])+/g,'').replaceAll(',','.')) * dinheiros) + ' ]'; break;} }},salarys);})()
change the favorite name as you want
click on the favorite that you saved it
the prompt will be showed, you have to put the cotation from usd today
hit enter again
now you can use the code whenever you want
enjoy
