# 🦠 Covid-19 in India Dashboard Analysis (Tableau)

## 📌 Project Overview

Is project me hum Tableau Desktop ki help se **Covid-19 in India Dashboard** banayenge. Dashboard banane ke liye hum total **6 Excel Datasets** aur **1 India State Spatial File (Shapefile)** ka use karenge.

Dashboard ka objective hai India ke Covid-19 data ko visually analyse karna taaki hum easily state-wise deaths, confirmed cases, cured cases, vaccination details, testing details, gender distribution aur age group analysis dekh sake.

---

# 📂 Datasets Used

Is project me total **6 datasets** aur **1 Spatial File** use hui hai.

| Dataset | Purpose |
|----------|----------|
| covid_19_india.xlsx | Covid Cases, Deaths, Map & Trend Analysis |
| covid_vaccine_statewise.xlsx | Vaccination Analysis |
| AgeGroupDetails.xlsx | Age Group Analysis |
| IndividualDetails.xlsx | Gender Analysis |
| ICMRTestingLabs.xlsx | Statewise Testing Labs |
| StatewiseTestingDetails.xlsx | Statewise Testing Report |
| India_State_Shapefile | India State Map |

---

# 📊 Dataset Explanation

## 1. covid_19_india.xlsx

Ye humara main dataset hai. Isme Covid-19 ke almost saare important details available hain.

### Important Columns

- Date
- State/Union Territory
- Confirmed
- Cured
- Deaths
- Country

### Is Dataset ka Use

- India Map
- Covid Cases Trend

---

## 2. covid_vaccine_statewise.xlsx

Is dataset me vaccination ki complete information available hai.

### Important Columns

- First Dose Administered
- Second Dose Administered
- Covishield
- Covaxin
- Sputnik V

### Is Dataset ka Use

- First vs Second Dose
- Vaccine Wise Analysis

---

## 3. AgeGroupDetails.xlsx

Ye dataset age group wise Covid cases batata hai.

### Important Columns

- Age Group
- Total Cases

### Is Dataset ka Use

Age Group Donut Chart

---

## 4. IndividualDetails.xlsx

Ye dataset gender wise Covid patient details batata hai.

### Important Columns

- Gender

### Is Dataset ka Use

Male vs Female Donut Chart

---

## 5. ICMRTestingLabs.xlsx

Ye dataset har state ke testing labs ki information rakhta hai.

### Important Columns

- State
- Lab Name

### Is Dataset ka Use

ICMR Testing Labs

---

## 6. StatewiseTestingDetails.xlsx

Ye dataset har state ki testing report batata hai.

### Important Columns

- State
- Positive
- Negative
- Total Samples

### Is Dataset ka Use

Statewise Testing Dashboard

---

## 7. India_State_Shapefile

Ye Spatial Dataset hai jiska use Tableau me India ka Map generate karne ke liye kiya gaya hai.

### Important Columns

- Name
- Type
- Geometry

---

# 📊 Worksheet 1

# 🗺️ Map : Total Death by State

Sabse pehle hum **covid_19_india.xlsx** ko Tableau me connect karenge.

Is dataset me bahut saare columns available hain jaise

- State/Union Territory
- Country
- Confirmed
- Cured
- Deaths

Ab is dataset ko Tableau me import kar lo.

Jaise hi dataset import hoga Tableau automatically Map create karne ki try karega, lekin ye India ke State Boundaries ko identify nahi kar payega.

Is problem ko solve karne ke liye hum India ka Spatial File import karenge.

## Import Spatial File

```
Data

↓

New Data Source

↓

Spatial File

↓

India_State_Shapefile
```

Is file me total 3 columns hain

- Name
- Type
- Geometry

Ab dubara

```
Map : Total Death by State
```

wali worksheet par aa jao.

Ab Blend Relationship create karenge.

```
Data

↓

Edit Blend Relationship

↓

Custom

↓

Add
```

Relationship

```
State/Union Territory

↓

Name
```

OK kar do.

Ab

```
Geometry
```

par Double Click karo.

Double Click karte hi India ka Map generate ho jayega.

Ab Data Source me

```
covid_19_india
```

select karo.

Ab

```
State/Union Territory

↓

Label
```

me daal do.

Isse Map par saare States aur Union Territories ke naam show hone lagenge.

Ab

```
Deaths

↓

Color
```

me daal do.

Ab har State ka Death Count color ke through show hone lagega.

Better visualization ke liye Color Palette ko

- Red
- Gold

kar do.

## Formatting

```
Format

↓

Shading

↓

Worksheet

↓

Grey
```

Map Background Dark karne ke liye

```
Map

↓

Background Map

↓

Dark
```

Title par click karo

```
Map : Total Death by State
```

Aur

- Bold
- White
- Center

kar do.

Uske baad

```
Format Title

↓

Border
```

add kar do.

✅ Worksheet 1 Complete.

---

# 📊 Worksheet 2

# Covid Cases by State

Is worksheet me hum Covid Cases ka Trend Analysis banayenge.

### Steps

Columns me

```
Date
```

daalo.

Date par Left Click karke usko

```
Exact Date
```

kar do.

Ab

```
Measure Names

↓

Filter
```

me jao.

Sirf ye 3 values select karo.

- Confirmed
- Cured
- Deaths

Ab

```
Measure Names

↓

Color
```

me daal do.

Aur

```
Measure Values

↓

Rows
```

me daal do.

Ab

```
SUM(Deaths)
```

ko bhi Rows me daalo.

Uske baad

```
Dual Axis
```

kar do.

Y-Axis par Double Click karke naam change kar do.

```
Confirmed & Cured
```

Ab line colors change karo.

- Confirmed → Green
- Cured → Orange
- Deaths → Red

Ab

```
State/Union Territory

↓

Filter
```

me laakar koi bhi State select kar lo.

Formatting

```
Format

↓

Shading

↓

Black
```

Aur Grid Lines remove kar do.

✅ Worksheet 2 Complete.

---

# 📊 Worksheet 3

# First vs Second Dose Administered

Ab

```
Data

↓

New Data Source

↓

covid_vaccine_statewise.xlsx
```

Import karo.

Worksheet ka naam rakho

```
First vs Second Dose Administered
```

Ab

```
Measure Names

↓

Filter
```

me jao.

None karo aur sirf ye select karo.

- First Dose Administered
- Second Dose Administered

Ab

```
Measure Values

↓

Columns
```

Aur

```
Measure Names

↓

Rows
```

Entire View kar do.

Grid Lines remove kar do.

Title ko

- Bold
- Center

kar do.

Aur Border add kar do.

✅ Worksheet 3 Complete.

---

# 📊 Worksheet 4

# Doses Administered by Vaccine

Same Dataset use karenge.

Worksheet ka naam rakho

```
Doses Administered by Vaccine
```

Measure Names Filter me jao.

None karo.

Sirf ye select karo.

- Covishield
- Covaxin
- Sputnik V

Ab

```
Measure Names

↓

Columns
```

Aur

```
Measure Values

↓

Rows
```

Entire View kar do.

Apni pasand ka color use kar lo.

Title ko Center aur Bold kar do.

Border add kar do.

✅ Worksheet 4 Complete.

---

# 📊 Worksheet 5

# Age Group Details

Ab

```
AgeGroupDetails.xlsx
```

Import karo.

Ab

```
Age Group

↓

Color
```

Marks ko

```
Pie
```

kar do.

Ab

```
Total Cases

↓

Size
```

me daal do.

Age Group ke according Pie Chart ban jayega.

Ab Columns me

```
0
```

likho.

Phir dubara

```
0
```

likho.

2 Pie Chart create ho jayenge.

Ab

```
SUM(0)(2)
```

ki values remove kar do.

Dusra Pie blank ho jayega.

Uski size thodi choti kar do.

Ab

```
Dual Axis
```

kar do.

Dono Pie overlap ho jayenge aur ek Donut Chart ban jayega.

Color aur Heading adjust kar lo.

✅ Worksheet 5 Complete.

---

# 📊 Worksheet 6

# Gender Without Missing Values

Ab

```
IndividualDetails.xlsx
```

Import karo.

Worksheet ka naam rakho.

```
Gender Without Missing Values
```

Ab

```
Gender

↓

Color
```

Aur Gender ko hi

```
Size
```

me daal do.

Gender par Right Click karke

```
Measure

↓

Count
```

kar do.

Ab Donut Chart banane ke liye wahi same process follow karo jo Age Group wale chart me kiya tha.

Agar Gender me

- M
- F

show ho raha ho to usko change kar do.

```
Gender

↓

Aliases
```

M → Male

F → Female

Formatting

```
Format

↓

Shading
```

Worksheet ka Background change kar lo.

**Note:** Kabhi-kabhi Formatting apply nahi hoti.

Dhyan rahe ki Formatting karte time niche

- Sheet
- Rows
- Columns

me se hamesha **Sheet** select hona chahiye.

✅ Worksheet 6 Complete.

---

# 📊 Worksheet 7

# ICMR Testing Labs in Each State

Ab

```
ICMRTestingLabs.xlsx
```

Import karo.

Fields use karo.

State

↓

Rows

Lab

↓

Columns

Ab Lab par Right Click karo.

```
Measure

↓

Count
```

Count(Lab) ko

```
Label
```

me daal do.

Formatting

```
Format

↓

Cell Size

↓

Taller
```

Ab

```
Rows
```

par Right Click karo.

```
Hide Field Labels for Rows
```

Axis Title remove kar do.

Bar Color Green kar do.

Formatting apni Dashboard Theme ke according kar lo.

✅ Worksheet 7 Complete.

---

# 📊 Worksheet 8

# Dashboard Title

Ab ek

```
Calculated Field
```

create karenge.

Search ke bagal wale arrow par click karo.

```
Create Calculated Field
```

Title do.

```
Covid-19 in India Dashboard Analysis
```

Is field ko

```
Text
```

me daal do.

Worksheet Title par click karo.

```
Hide Title
```

kar do.

Formatting

- Center
- Bold
- White
- Black Background

✅ Worksheet 8 Complete.

---

# 📊 Worksheet 9

# Statewise Testing Details

Ab

```
StatewiseTestingDetails.xlsx
```

Import karo.

Worksheet ka naam rakho.

```
Statewise Testing Details
```

Ab

```
Measure Names

↓

Filter
```

me jao.

Sirf ye select karo.

- Positive
- Negative
- Total Samples

Ab

```
Measure Values

↓

Rows
```

Aur

```
State

↓

Columns
```

me daal do.

Apni Dashboard Theme ke according Colors aur Formatting kar lo.

Grid Lines remove kar do.

Border add kar do.

Title ko Bold aur Center kar do.

✅ Worksheet 9 Complete.

---

# 🎯 Final Dashboard

Ab saari Worksheets complete ho chuki hain.

Ab ek naya Dashboard create karo aur saari Worksheets ko arrange karke ek professional Covid-19 Dashboard bana lo.

Dashboard me include honge:

- 🗺️ Map : Total Death by State
- 📈 Covid Cases by State
- 👥 Gender Without Missing Values
- 👶 Age Group Details
- 💉 First vs Second Dose Administered
- 💊 Doses Administered by Vaccine
- 🏥 ICMR Testing Labs
- 🧪 Statewise Testing Details

Finally Dashboard ki Formatting same Theme me rakho.

- Dark Background
- White Titles
- Borders
- Proper Alignment
- Consistent Colors

Iske baad Dashboard publish ya save kar do.

---
**Happy Learning! 🚀**