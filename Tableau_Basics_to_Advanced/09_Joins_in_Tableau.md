# 🔗 Joins in Tableau

## 📌 What are Joins?

**Join** ek technique hai jiska use **2 ya usse zyada tables ko kisi common column (Key)** ki help se combine karne ke liye kiya jata hai.

Simple words me,

> Agar data alag-alag Excel files ya database tables me stored ho aur hume un sabko ek hi table ki tarah use karna ho, to hum **Join** ka use karte hain.

---

## 🎯 Why Do We Use Joins?

Real-life me data kabhi bhi ek hi file me nahi hota.

Example:

- Employee Details → Demographics.xlsx
- Employee Job Title → JobTitle.xlsx
- Employee Salary → Salary.xlsx

Agar hume kisi employee ki **Age + Gender + Job Title + Salary** ek saath dekhni ho, to pehle in tino tables ko join karna padega.

---

# 🔑 Common Key

Join tabhi possible hota hai jab dono tables me koi **Common Column (Key)** ho.

Example:

```
EmployeeID
```

Ye tino tables me available hai, isliye isi ke basis par join kiya jayega.

---

# Types of Joins in Tableau

## 1️⃣ Inner Join

### Definition

Sirf wahi rows return karta hai jo **dono tables me match karti hain.**

### Example

Table A

| EmployeeID |
| ---------: |
|       1001 |
|       1002 |
|       1003 |

Table B

| EmployeeID |
| ---------: |
|       1002 |
|       1003 |
|       1004 |

Output

| EmployeeID |
| ---------: |
|       1002 |
|       1003 |

✅ Sirf common records.

---

## 2️⃣ Left Join

Left table ka **saara data** aata hai.

Right table ka sirf matching data.

Agar match na mile to **NULL** aata hai.

---

## 3️⃣ Right Join

Right table ka **saara data** aata hai.

Left table ka sirf matching data.

Match na hone par NULL show hota hai.

---

## 4️⃣ Full Outer Join

Dono tables ka **poora data** aata hai.

Matching rows combine ho jati hain.

Non-matching rows me NULL show hota hai.

---

# Summary Table

| Join Type | Output |
| ---------- | ------ |
| Inner Join | Sirf Matching Records |
| Left Join | Left Table + Matching Right |
| Right Join | Right Table + Matching Left |
| Full Outer Join | Dono Tables ka Complete Data |

---

# 📂 Dataset Used

Is tutorial me humare paas **3 Excel Sheets** thi.

## 1. Demographics

Isme employee ki personal information thi.

Columns:

- EmployeeID
- EmployeeName
- EmployeeAge
- EmployeeGender

---

## 2. JobTitle

Isme employee ka designation tha.

Columns:

- EmployeeID
- EmployeeName
- JobTitle

---

## 3. Salary

Isme employee ki salary thi.

Columns:

- EmployeeID
- EmployeeSalary

---

# 🛠️ How to Join Tables in Tableau

## Step 1

Tableau open karein.

Connect to Excel se apni workbook import karein.

---

## Step 2

Workbook open hone ke baad left side me tino sheets dikhengi.

- Demographics
- JobTitle
- Salary

---

## Step 3

Sabse pehle **Demographics** sheet ko drag karke canvas par drop karein.

Ye hamari primary table hogi.

** Demographics** pr click krke open select kr lo


### Step 4

 Uske baad **JobTitle** sheet ko Demographics ke paas drag kiya.
 Tableau ne automatically common field (`EmployeeID`) detect kar liya.
 Join type ko **Inner Join** select kiya.



### Step 5


 Isi tarah **Salary** sheet ko bhi drag karke **Inner Join** select kiya.
 

> **Note:** Agar dono tables me common column ka naam aur datatype same ho, to Tableau automatically join condition detect kar leta hai. Isliye hume manually join condition select karne ki zarurat nahi padti.


## Step 6

Ab tino tables successfully join ho chuki hain.

Aap chahe to is joined table ka naam bhi change kar sakte hain.

Example:

```
Employee_Data
```

ya

```
Employee_Details
```

---

## Step 7

Ab **Go to Worksheet** par click karein.

Ab joined table ke saare fields ek hi jagah available honge.

Jaise:

- EmployeeID
- EmployeeName
- EmployeeAge
- EmployeeGender
- JobTitle
- EmployeeSalary

Ab in sab fields ko use karke koi bhi visualization bana sakte hain.

---

# 📊 Result

Inner Join ke baad hume sirf wahi employees mile jinka data tino tables me available tha.

Example:

| EmployeeID | Name | Age | Gender | Job Title | Salary |
| ---------: | ---- | --- | ------ | --------- | -----: |
| 1001 | Jim Halpert | 35 | Male | Salesman | 45000 |
| 1002 | Pam Beesly | 35 | Female | Receptionist | 35000 |
| 1003 | Dwight Schrute | 37 | Male | Assistant to the Regional Manager | 65000 |

---

# 💡 Real-Life Uses of Joins

Joins ka use bahut common hai:

- Employee Information + Salary
- Customer Details + Orders
- Students + Marks
- Product Details + Sales
- Hospital Patient + Medical Records
- Bank Customer + Transactions

---

# ✅ Advantages

✔ Multiple tables ko ek saath analyze kar sakte hain.

✔ Duplicate data maintain karne ki zarurat nahi hoti.

✔ Data analysis aur reporting easy ho jati hai.

✔ Different sources ke data ko combine kar sakte hain.

