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
### Task: Create a New Data Policy
**1. Navigate to Data Policies** <br>
- **All > DXC Technology Devices > Device Inventory** <br>
- In the **Asset Recovery Request** table, hover over any column until an icon with three verticle dots appear. Click on it --> **Configure > Data Policies** <br>

![](https://github.com/CodeWithLuwam/August-5-Data-Policies/blob/main/Images/Configure%20Data%20Policies.png?raw=true) <br>

*These are the data policies that are corresponding to our tables specifically, right now we dont have any, thats why the menu is empty.* <br>
![](https://github.com/CodeWithLuwam/August-5-Data-Policies/blob/main/Images/Data%20Policies%20in%20Current%20Table.png?raw=true) <br>

**2. Create the Data Policy** 
- Click **New**.
- The table name will auto-populate <br>
*Note: If you open Data Policies directly from the All menu, you’ll need to manually select the table. Opening from the column menu fills it in automatically.*
![](https://github.com/CodeWithLuwam/August-5-Data-Policies/blob/main/Images/Auto%20Populated%20Table%20Name.png?raw=true) <br>
- **Apply to all data types** by checking:
    - Apply to Import Sets
    - Apply to SOAP (API protocol)
    - Use as a UI Policy on Client (functions like a UI Policy but doesn’t create one separately)
![](https://github.com/CodeWithLuwam/August-5-Data-Policies/blob/main/Images/Apply%20to%20import%20sets%20Apply%20to%20SOAP%20Uses%20as%20UI%20Policy%20on%20client.png?raw=true)  <br>

**3. Set Conditions**<br>
- Asset Type is Laptop <br>
![](https://github.com/CodeWithLuwam/August-5-Data-Policies/blob/main/Images/Condition%20Asset%20Type%20is%20Laptop.png?raw=true) <br>

**4. Save** <br>
- After saving, the **Data Policy Rules** related list will appear.<br>
![](https://github.com/CodeWithLuwam/August-5-Data-Policies/blob/main/Images/Data%20Policy%20Rules%20Menu%20Appears.png?raw=true) <br>

**5. Add Data Policy Rules**
- Click **New** button in that Data Policy Rules list. <br>
- Make the following fields Mandatory when the Asset Type is Laptop: <br>
    - Laptop Serial Number <br>
    - Urgency <br>
    - Employee <br>
- Save each rule and repeat for all required fields.
![](https://github.com/CodeWithLuwam/August-5-Data-Policies/blob/main/Images/Pick%20Field%20Name%20Laptop%20Serial%20Number.png?raw=true) <br>
Submitting will bring us back to the Data Policy Rule record and we can see the Field name we just added in the Data Policy Rules menu. <br>
![](https://github.com/CodeWithLuwam/August-5-Data-Policies/blob/main/Images/Confirm%20New%20Field%20Name%20Added.png?raw=true) <br>

---

### Testing

1. Navigate to: **All  > DXC Technology Devices > Device Inventory -->** *(links to Asset Recovery Request table)* <br>
2. Create a new record <br>
3. Set **Asset Type** to **Laptop** <br>
4. Confirm that **Laptop Serial Number**, **Urgency** and **Employee** are now mandatory. <br>
![](https://github.com/CodeWithLuwam/August-5-Data-Policies/blob/main/Images/Asset%20Type%20Triggers%20Madatory%20Fields.png?raw=true) <br>

