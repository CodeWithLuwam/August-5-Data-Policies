# August-5-Data-Policies

**Activity** <br>

At DXC Tech, you've noticed that many asset records are created not just through the UI, but also through import sets or external integrations. However, when the asset being recovered is a laptop, it's critical to ensure a serial number is always provided, regardless of how the data enters the system. <br>

To enforce this across all entry methods, you've been asked to implement a Data Policy that ensures laptops always have a valid serial number, urgency and employee even if the data comes in via an integration or spreadsheet import.<br>

**Task**: <br>
**Create a New Data Policy** <br>
- Apply to all data types
- Save <br>

**Add Data Policy Rules** <br>

Make sure the following fields are mandatory:
- laptop serial number
- Urgency
- employee

---

All > DXC Technology Devices > Device Inventory <br>
In the Asset Recovery Request table, go to any column, hover until three verticle dots appear. Then click on it, Configure > Data Policies <br>
![](https://github.com/CodeWithLuwam/August-5-Data-Policies/blob/main/Images/Configure%20Data%20Policies.png?raw=true) <br>
These are the data policies that are corresponding to our tables specifically <br>
right now we dont have any, thats why the menu is empty. <br>
![](https://github.com/CodeWithLuwam/August-5-Data-Policies/blob/main/Images/Data%20Policies%20in%20Current%20Table.png?raw=true) <br>
When we click New, we dont have to fill out the table name, it automatically fills it out for us. <br>
If we were to just look up data policies in the All menu and create new, we would have to specify the table. <br>
![](https://github.com/CodeWithLuwam/August-5-Data-Policies/blob/main/Images/Auto%20Populated%20Table%20Name.png?raw=true) <br>
To the right is where all the data policy is going to apply

And then the next step was to apply all the data types.  These are where the datapolicy is gonna apply. We have: <br> 
- Apply to import sets,
- Apply to SOAP (an protocol when we're using the APIs)
- Use as a UI Policy on client. (So since it's doing the same thing as a Ui policy, we could also activate it from here. It technically won't create a new ui policy. But it's a way to achieve the same outcome. ) <br>
![](https://github.com/CodeWithLuwam/August-5-Data-Policies/blob/main/Images/Apply%20to%20import%20sets%20Apply%20to%20SOAP%20Uses%20as%20UI%20Policy%20on%20client.png?raw=true)  <br>
The condition will be: <br>
Asset Type is Laptop <br>
![](https://github.com/CodeWithLuwam/August-5-Data-Policies/blob/main/Images/Condition%20Asset%20Type%20is%20Laptop.png?raw=true) <br>
We Save and then now we have our Data Policy Rules menu, which we previously did not have <br>
![](https://github.com/CodeWithLuwam/August-5-Data-Policies/blob/main/Images/Data%20Policy%20Rules%20Menu%20Appears.png?raw=true) <br>
Click the New button in that menu. <br>
So we said that when laptop is the Asset Type, the Laptop Serial Number, Urgency and Employee are all mandatory.
![](https://github.com/CodeWithLuwam/August-5-Data-Policies/blob/main/Images/Pick%20Field%20Name%20Laptop%20Serial%20Number.png?raw=true) <br>
Submitting will bring us back to the Data Policy Rule record and we can see the Field name we just added in the Data Policy Rules menu. <br>
![](https://github.com/CodeWithLuwam/August-5-Data-Policies/blob/main/Images/Confirm%20New%20Field%20Name%20Added.png?raw=true) <br>
Repeat the process for Urgency and Employee. <br>

### Test

All  > DXC Technology Devices > Device Inventory --> links to (Asset Recovery Request table) <br>
Create New <br>
Set the Asset Type Laptop - condition to be triggered, we see then that *Laptop Serial Number, *Urgency and *Employee <br>
![](https://github.com/CodeWithLuwam/August-5-Data-Policies/blob/main/Images/Asset%20Type%20Triggers%20Madatory%20Fields.png?raw=true) <br>

