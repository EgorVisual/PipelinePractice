[![Build Status](https://dev.azure.com/alekseevap/falameev/_apis/build/status/EgorVisual.PipelinePractice?branchName=master)](https://dev.azure.com/alekseevap/falameev/_build/latest?definitionId=12&branchName=master)

# Отчет о работе с Azure Pipelines.
Данный репозиторий был содан с целью первичного взаимодествия с Azure Pipelines.
На основе простого приложения, выполняющего функции калькулятора, был создан примитивный веб-интерфейс, а также созданы функциональные и программные тесты. 
Результаты прохождения программных тестов в рамках Pipeline: 

![img_1.png](assets/UnitTests.png)

Веб-приложение в Azure DevOps:

![img.png](assets/AppAzure.png)

В ходе развертвания веб-приложения в Azure DevOps мы получили ссылку на него:

https://falameev-web.azurewebsites.net/

Перейдя по ссылке мы попадаем на страницу с нашим веб-приложением: 

![img.png](assets/Web-appStarts.png)

Для взаимодействия с приложением слеует в поисковой строке к запросу приписать:
Функцию для исполнения приложением:
1. /add
2. /multiply
3. /subtract
4. /divide

И значения для обработки данной функцией в следующем виде:

/<Значение 1>&<Значение 2>

Пример результатов взаимодествия с веб-приложением:

![img.png](assets/1ExampleWeb-app.png)

![img.png](assets/2ExampleWeb-app.png)

![img.png](assets/3ExampleWeb-app.png)

Настроенный пайплайн в Azure DevOps для запуска релиза:

![img.png](assets/Pipeline.png)

Результаты прохождения функциональных тестов и релиз в Azure DevOps:

![img.png](assets/ReleaseWeb-app.png)

В результате прохождения всех тестов и выпуска приложения репозиторий гитхаба бул отмечен зеленной галочкой: 

![img.png](assets/GreenAccess.png)
