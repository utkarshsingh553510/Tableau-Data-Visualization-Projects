# 📈 Line Chart in Tableau

Line Chart ka use **time ke saath data me hone wale changes (Trends)** ko dikhane ke liye kiya jata hai.

> Ye sabse useful chart hai jab hume kisi value ka increase ya decrease over time dekhna ho.

---

# Example 1: Global Sales by Year

### Step 1
**Year** ko **Columns Shelf** me drag & drop karein.

👉 Ye X-Axis ban jayega.

### Step 2
**Global Sales** ko **Rows Shelf** me drag & drop karein.

👉 Tableau automatically **SUM(Global Sales)** calculate karega aur Y-Axis bana dega.

### Step 3
**Show Me** panel se **Line Chart** select karein.

---

## Output

Is chart me har **Year** ke according total **Global Sales** dikhai deti hai.

### Observation

- 1980–1995 tak sales kam thi.
- 1996 ke baad sales rapidly increase hui.
- 2008–2009 ke aas-paas highest sales dekhne ko mili.
- Uske baad sales gradually decrease hone lagi.

---

## 📌 Real-Life Use

Agar kisi company ki yearly sales dekhni ho to Line Chart sabse best choice hota hai.

Example:
- Amazon Sales by Year
- Company Revenue by Year
- Temperature by Month
- Population Growth

---

# Example 2: Global Sales by Year and Genre

Ab hum chart me **Genre** bhi add karte hain.

### Step 1

Year → Columns

### Step 2

Global Sales → Rows

### Step 3

Genre ko **Marks Card** ke **Color** ya **Detail** option me drag karein.



---

## Output

Ab ek line ki jagah har **Genre** ke liye alag-alag line create ho jayegi.

Example:

- Action
- Sports
- Racing
- Adventure
- Shooter
- Puzzle

Har Genre ki sales alag line se represent hogi.

---

## 📊 Is Chart se Kya Pata Chalta Hai?

- Kis Genre ki sales sabse zyada thi.
- Kis Year me kis Genre ne best perform kiya.
- Different Genres ka trend compare kar sakte hain.

---

## 💡 Difference Between Both Charts

| First Chart | Second Chart |
|-------------|--------------|
| Sirf Year vs Global Sales | Year vs Global Sales + Genre |
| Ek hi line hoti hai | Multiple lines hoti hain |
| Overall sales trend dikhata hai | Har Genre ka trend compare karta hai |

---

## ✅ Summary

- **Columns** → Year
- **Rows** → SUM(Global Sales)
- **Chart Type** → Line Chart
- **Genre (Color/Detail)** → Multiple lines create karta hai.
- Line Chart ka main use **Trend Analysis** aur **Time Series Analysis** ke liye hota hai.





# 📊 Bar Chart in Tableau

Bar Chart ka use **alag-alag categories ki values compare** karne ke liye kiya jata hai.

---

## Example

**Question:** Kis Genre ki Global Sales sabse zyada hai?

### Steps

1. Genre → Columns
2. Global Sales → Rows
3. Show Me → **Bar Chart**

---

## Output

Har Genre ke liye ek alag Bar banega.

Example:

- Action
- Sports
- Racing
- Shooter
- Puzzle

Jis Genre ki sales sabse zyada hogi uska bar sabse bada hoga.

---

## Use Cases

- Product Sales Comparison
- Student Marks Comparison
- Company Revenue Comparison
- Game Genre Sales Comparison

---

## Advantages

✅ Categories compare karna easy hota hai.

✅ Sabse high aur lowest value easily identify ho jati hai.

---

## Summary

- Columns → Genre
- Rows → SUM(Global Sales)
- Chart → Bar Chart
- Purpose → Category Comparison








# 🥧 Pie Chart in Tableau

Pie Chart ka use **Part-to-Whole Relationship** dikhane ke liye hota hai.

Ye batata hai ki total value me har category ka kitna contribution hai.

---

## Example

**Question:** Total Global Sales me har Platform ka kitna contribution hai?

### Steps

1. Platform → Color
2. Global Sales → Angle
3. Show Me → Pie Chart

---

## Output

Har Platform pie ka ek slice ban jayega.

Example:

- PS2 → 22%
- Xbox → 15%
- Wii → 18%
- PC → 10%

---

## Real-Life Uses

- Market Share
- Browser Usage
- Population Distribution
- Sales Contribution

---

## Advantages

✅ Percentage easily samajh aati hai.

✅ Part-to-Whole relationship dikhata hai.

---

## Limitation

Agar categories bahut zyada ho (10–15+) to Pie Chart confusing ho jata hai.

Us situation me **Bar Chart** use karna better hota hai.

---

## Summary

- Dimension → Platform
- Measure → Global Sales
- Chart → Pie Chart
- Purpose → Percentage / Contribution Analysis








# 📈 Advanced Line Chart with Filters in Tableau

Is visualization me humne sirf Year aur Global Sales hi nahi, balki **Genre**, **Platform Filter** aur **Data Labels** bhi use kiye hain.

---

## 🎯 Objective

Alag-alag **Game Genres** ki **Global Sales** ko Year-wise compare karna aur sirf selected Platforms ka data dekhna.

---

## 🛠️ Steps

### Step 1

**Year** ko **Columns Shelf** me drag karein.

👉 Ye X-Axis ban jayega.

---

### Step 2

**Global Sales** ko **Rows Shelf** me drag karein.

👉 Tableau automatically **SUM(Global Sales)** calculate karega.

---

### Step 3

**Genre** ko **Marks Card → Color** me drag karein.

👉 Har Genre ke liye alag color ki line ban jayegi.

---

### Step 4

**Platform** ko **Filters Shelf** me drag karein.

👉 Ab user sirf selected gaming platforms ka data dekh sakta hai.
pahele All select kr lo then uske baad jisko man hai usko exclude ya include krke dekh skte ho 
Example:

- PS2
- PS3
- Xbox
- Wii
- PC

---

### Step 5

**Global Sales** ko **Label** me drag karein.

👉 Important points ke upar sales values (jaise 114.8, 90.3, 59.1) display hone lagti hain.

---

## 📊 Output

Chart me:

- X-Axis → Year
- Y-Axis → Global Sales
- Different Colors → Different Genres
- Right Side Filter → Platform Selection
- Labels → Sales Values

---

## 🔍 Analysis

Is chart se hum easily dekh sakte hain:

- Kis Genre ki sales sabse zyada thi.
- Kis Year me peak sales hui.
- Kis Platform ko select karne par trend kaise change hota hai.
- Different Genres ka performance compare kar sakte hain.

---

## 💡 Real-Life Example

Agar kisi company ko sirf **PlayStation Games** ki sales dekhni ho to Platform Filter me sirf **PS2, PS3, PS4** select kar sakte hain.

Agar sirf **PC Games** ka analysis karna ho to sirf **PC** select karna hoga.

Isse visualization dynamically update ho jayega.

---

## 📌 Features Used

- ✅ Line Chart
- ✅ Color Encoding (Genre)
- ✅ Filter (Platform)
- ✅ Labels (Global Sales)
- ✅ Trend Analysis
- ✅ Interactive Visualization

---
> **Note:** Tableau me Filters visualization ko interactive bana dete hain. User filter change karke real-time me alag-alag data ka analysis kar sakta hai, bina naya chart banaye.










# 📊 Bar Chart with Sorting in Tableau

Is example me humne **Genre-wise Global Sales** ka Bar Chart banaya hai aur data ko **Descending Order** me sort kiya hai.

---

## 🎯 Objective

Ye dekhna ki kis **Game Genre** ki Global Sales sabse zyada aur sabse kam hai.

---

## 🛠️ Steps

### Step 1

**Genre** ko **Columns Shelf** me drag karein.

👉 Ye X-Axis ban jayega.

---

### Step 2

**Global Sales** ko **Rows Shelf** me drag karein.

👉 Tableau automatically **SUM(Global Sales)** calculate karega.

---

### Step 3

**Show Me** panel se **Bar Chart** select karein.

---

### Step 4

**Genre** ko **Color** me drag karein.

👉 Har Genre ka bar alag color me dikhai dega.

---

### Step 5 (Sorting)

Toolbar me **Sort Descending (↓)** button par click karein.

👉 Bars highest sales se lowest sales ke order me arrange ho jayenge.

---

## 📊 Output

Chart me sabhi Genres ki Global Sales compare hoti hai.

Example:

- 🥇 Action → Highest Sales
- 🥈 Sports
- 🥉 Shooter
- Role-Playing
- Platform
- Misc
- Racing
- Fighting
- Simulation
- Puzzle
- Adventure
- Strategy → Lowest Sales

---

## 🔍 Analysis

Is chart se hum easily pata laga sakte hain:

- Kis Genre ki sales sabse zyada hai.
- Kis Genre ki sales sabse kam hai.
- Genres ki ranking kya hai.
- Data ko descending ya ascending order me compare kar sakte hain.

---




## 🔄 Sorting in Tableau

Tableau me sorting ke do options hote hai and ye upar toolbar me hota hai jaha pr File,Data,Worksheet,Dashboard ..etc hota hai uske niche 

### 🔽 Descending Sort

Data ko **Highest → Lowest** order me arrange karta hai.

Example:

```
Action → 1750
Sports → 1320
Shooter → 1030
...
Strategy → 180
```

---

### 🔼 Ascending Sort

Data ko **Lowest → Highest** order me arrange karta hai.

Example:

```
Strategy → 180
Adventure → 250
Puzzle → 260
...
Action → 1750
```

---

## 💡 Real-Life Uses

Sorting ka use bahut common hai:

- Top Selling Products
- Highest Revenue Companies
- Best Performing Students
- Most Popular Movie Genres
- State-wise Population
- Country-wise GDP

---

## ✅ Advantages

- Highest aur Lowest values instantly identify ho jati hain.
- Data compare karna easy ho jata hai.
- Reports aur Dashboards zyada readable ban jate hain.


> **Interview Tip:** Dashboard me Category Comparison ke liye hamesha **Descending Sort** use karna best practice mana jata hai, kyunki sabse important values sabse pehle dikhai deti hain.





