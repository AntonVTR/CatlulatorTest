**Bug Name:** Некорректная обработка больших значений  
**Build Number:** 1.225.1.1-1819727  
**Environment:** Android virtual device Android 9.0 (Google APIs)  
**Description:** При попытке выплнить операцию со значением больше 10e7, в результате возникает ошибка в отображаемом значании   

**Steps To Reproduce:**  
1. Запустить приложение AndroidSampleApp  
2. В поле ввода 1 ввести 3333333333333333333333333.25   
3. В поле ввода 2 ввести 2222222222222222222222222  
4. Нажать на "+"  
5. Резульат 3333333283417967500000000.00 + 2222222188945311600000000.00 = 5555555184132903000000000.00  

**Expected Result:**  
3333333333333333333333333.25 + 2222222222222222222222222.00 = 5555555555555555555555555.25  