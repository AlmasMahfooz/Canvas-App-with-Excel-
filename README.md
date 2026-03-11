# Canvas-App-with-Excel-

Below is the screen shot of excel file for which I am going to create canvas app so user data can be insert /update from front end.


![Uploading image.png…](https://github.com/AlmasMahfooz/Canvas-App-with-Excel-/blob/main/ScreenShots/excel1.png)


I choose recommended setting while setting datasource for my application , screen shot below.


![Uploading image.png…](https://github.com/AlmasMahfooz/Canvas-App-with-Excel-/blob/main/ScreenShots/excel2.png)


Once Datasource added to Application new column will be added to the excel.


![Uploading image.png…](https://github.com/AlmasMahfooz/Canvas-App-with-Excel-/blob/main/ScreenShots/excel3.png)


With the help of Gallery control I am filtering to table and get data back to gallery and then Form. I turned this gallery visible property falso as it is just to help the processes.

<code> If(CountRows(If(TextInput1.Text<>Blank(),Filter(Table1,EmployeeID=TextInput1.Text)))>0, Filter(Table1,EmployeeID=TextInput1.Text)) </code>


![Uploading image.png…](https://github.com/AlmasMahfooz/Canvas-App-with-Excel-/blob/main/ScreenShots/excel4.png)


Form's Item property is set as Gallery.Selected.
And below are other formulas for the various properties.
Also the Default property DataCardValue of Employe is set as TextInput1.Text


![Uploading image.png…](https://github.com/AlmasMahfooz/Canvas-App-with-Excel-/blob/main/ScreenShots/excel5.png)


The DefaultMode propert of Form is set as below
If(CountRows(If(TextInput1.Text<>Blank(),Filter(Table1,EmployeeID=TextInput1.Text)))>0,FormMode.Edit,FormMode.New)



And finally the save button code is like below.


![Uploading image.png…](https://github.com/AlmasMahfooz/Canvas-App-with-Excel-/blob/main/ScreenShots/excel6.png)


