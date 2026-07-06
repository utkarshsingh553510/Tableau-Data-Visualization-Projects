# 🗺️ Creating Your First Visualization in Tableau (Map Chart)

Ab tak humne Tableau interface aur basic charts (Bar, Line, Pie) dekh liye hain. Ab hum ek naya dataset use karke apna **pehla Map Visualization** banayenge.

---

# 📂 Dataset Used

Is example me humne **Starbucks Locations Worldwide** dataset use kiya hai.

Dataset me kuch important columns the:

- Brand
- Store Name
- Country
- State/Province
- City
- Street Address
- Latitude
- Longitude
- Ownership Type

Ye dataset geographical data contain karta hai, isliye ispar Map Visualization banana bahut easy hota hai.

---

# 🌍 Why Map Chart?

Jab bhi data kisi location se related ho, jaise:

- Country
- State
- City
- Latitude
- Longitude

to Tableau automatically us data ko map par plot kar sakta hai.

Map Chart ki help se hum easily dekh sakte hain ki stores ya locations duniya me kahan-kahan present hain.

---

# 🛠️ Steps to Create a Map Visualization

### Step 1

CSV dataset ko Tableau me connect karein.

---

### Step 2

Worksheet open karein.

---

### Step 3

Data Pane se **State/Province** (ya Country/City) field par **double-click** karein.

Ya us field ko worksheet me drag & drop karein.

---

### Step 4

Tableau automatically generated fields create kar deta hai.

- **Latitude (generated)**
- **Longitude (generated)**

Aur ek Map Visualization create ho jata hai.


Columns-> Latitude

Rows -> Longitude 

Marks -> City/State

---

# 📍 Output

Ab map par har State/Province ya City ek point ke roop me show hogi.

Har point Starbucks Store ki location ko represent karta hai.

Isse hum easily dekh sakte hain ki kis area me kitne stores hain.

---

# 🎨 Customize the Map

Map Banne ke baad Marks Field me Map dikhega uspr click kro 

Map banne ke baad hum **Marks Card** ki help se usko aur attractive bana sakte hain.

### Size

Marks Card → **Size**

Is option se map par dikhne wale circles (Marks) ka size bada ya chhota kar sakte hain.

👉 Bade circles important locations ko highlight karne me help karte hain.

---

### Color

Marks Card → **Color**

Alag-alag Country, State ya Ownership Type ko different colors me show kar sakte hain.

---

### Label

Marks Card → **Label**

Store Name ya City ka naam map par show kar sakte hain.

---

### Tooltip

Marks Card → **Tooltip**

Mouse hover karne par Store Name, City, Country aur baaki information show hoti hai.

---

# 📌 Real-Life Uses

Map Visualization ka use bahut jagah hota hai.

Examples:

- Starbucks Store Locations
- Amazon Delivery Centers
- Zomato Restaurant Locations
- Hospital Locations
- Bank Branches
- Crime Analysis
- Sales by Country
- Population Distribution

---

# ✅ Advantages

✔ Geographical data ko visualize karna easy hota hai.

✔ Store distribution easily samajh aata hai.

✔ High-density aur low-density areas identify kar sakte hain.

✔ Business expansion ke liye useful insights milte hain.

---

# 📝 Summary

- Dataset → Starbucks Locations Worldwide
- Double-click → State/Province (ya Country/City)
- Tableau automatically Latitude & Longitude generate karta hai.
- Result → Interactive Map Visualization
- Marks Card ki help se Size, Color, Label aur Tooltip customize kar sakte hain.

> **Note:** Tableau tabhi Map automatically banata hai jab dataset me Geographic fields (Country, State, City, Latitude ya Longitude) available hon.