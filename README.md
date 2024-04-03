# sit323--737-2024-t1-prac4p

Getting started:
- git clone <repository>
- npm install 
- node calculatorwithlogger.js 
- in web browser, go to one of the following locations: 

localhost:3040/${action}?n1=${n1}&n2=${n2}
Substitutions:
${action} with either add, subtract, multiply or divide 
${n1} and ${n2} with numbers. 

Eg - 
Addition: ${n1} + ${n2}
localhost:3040/add?n1=3&n2=4
Expected result: 7

Subtract: ${n1} - ${n2}
localhost:3040/sub?n1=3&n2=4
Expected result: -1

Multiplication: ${n1} * ${n2}
localhost:3040/mult?n1=3&n2=4
Expected result: 12

Divison: ${n1} / ${n2}
localhost:3040/div?n1=3&n2=4
Expected result: 0.75


Notes:
Each API endpoint (/add, /sub, /mult and /div) refer to the same error handling function (specifically errorHandling() here) which validates numbers using  validateNumbers(). For this to work, each end point must pass in their operation name.
This set up allows for specific edge cases (such as dividing by zero) to be resolved in the number validation/error handling functions. It also means that further adjustments (such as including additional operations) can be implemented with their specifics quite easily. 