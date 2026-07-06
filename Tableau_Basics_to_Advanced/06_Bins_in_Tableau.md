# 📦 Bins in Tableau

## 📌 What are Bins?

**Bins** Tableau ka ek feature hai jo **continuous numerical data ko equal-sized groups (intervals)** me divide karta hai.

Simple words me:

> **Bins ka matlab hai numerical values ko chhote-chhote groups (buckets) me convert karna, taaki data ko analyze karna aur visualize karna easy ho jaye.**

---

## 💡 Real-Life Example

Maan lo kisi class me students ke marks hain:

```
32, 35, 38, 41, 45, 48, 52, 55, 59
```

Agar hum **Bin Size = 10** rakhte hain, to Tableau automatically groups bana dega.

| Bin | Values |
|------|---------|
| 30–39 | 32, 35, 38 |
| 40–49 | 41, 45, 48 |
| 50–59 | 52, 55, 59 |

👉 Isse individual values dekhne ki jagah groups ka analysis karna easy ho jata hai.

---

# 🎮 Example: Video Game Sales Dataset

Humare dataset me **Year** ek numerical field hai.

Agar hum har ek year alag-alag analyze karein to chart bahut bada aur complex ho sakta hai.

Isliye hum **Bins** ka use karke Years ko groups me divide karte hain.

Example:

**Bin Size = 5**

To Tableau automatically groups bana dega.

| Year | Year (Bin) |
|------|------------|
| 1980 | 1980–1984 |
| 1985 | 1985–1989 |
| 1990 | 1990–1994 |
| 1995 | 1995–1999 |
| 2000 | 2000–2004 |
| 2005 | 2005–2009 |
| 2010 | 2010–2014 |
| 2015 | 2015–2019 |

Ab har year ki jagah 5-5 years ka ek group ban jayega.

---

# 🛠️ How to Create Bins in Tableau

### Step 1

Data Pane me **Year** field par Right Click karein.

### Step 2

**Create → Bins** select karein.

### Step 3

Ek dialog box open hoga.

**Size of Bins** me value enter karein.

Example:

```
5
```

Matlab har Bin me **5 Years** honge.

### Step 4

**OK** par click karein.

---

## Output

Data Pane me ek naya field create ho jayega.

```
Year (Bin)
```

Ye Tableau ka automatically generated field hota hai.

> **Note:** Bin create hone ke baad **Year (Bin)** ek **Dimension (Categorical Field)** ki tarah behave karta hai, kyunki ab individual years ki jagah groups (categories) ban chuki hoti hain.

---

# 📊 Creating Visualization Using Bins

Humne visualization me:

- **Year (Bin)** → Columns
- **SUM(Global Sales)** → Rows
- **Genre** → Color

use kiya.

Isse ek **Stacked Bar Chart** create hua.

---

## 📈 Output Analysis

Ab hum easily dekh sakte hain:

- Kis **5-Year Group** me sabse zyada Global Sales hui.
- Kis **Genre** ka contribution sabse zyada tha.
- Different Genres ki sales ko compare kar sakte hain.
- Long-term sales trend ko samajhna easy ho jata hai.

Example:

- **2000–2004** me sales highest thi.
- Is period me **Action** aur **Sports** Genre ka contribution sabse zyada tha.

---

# 🎯 Advantages of Bins

✅ Large numerical data ko groups me convert karta hai.

✅ Data ko samajhna easy ho jata hai.

✅ Histogram aur Stacked Bar Chart banane me useful hai.

✅ Trend analysis aur distribution analysis me help karta hai.

---

# 📌 When Should We Use Bins?

Bins ka use tab karte hain jab:

- Numerical data bahut zyada ho.
- Data ko groups me divide karna ho.
- Distribution dekhna ho.
- Histogram banana ho.
- Continuous data ko categorical form me convert karna ho.

---

# 📝 Summary

| Concept | Description |
|---------|-------------|
| Bins | Numerical data ko equal-sized groups me divide karna |
| Bin Size | Har group me kitni values ya range hogi |
| Year (Bin) | Year ka grouped version |
| Type | Dimension (Categorical) |
| Use | Histogram, Bar Chart, Distribution Analysis, Trend Analysis |

---

## 💡 Interview Point

> **Bins are used to convert continuous numerical data into equal-sized categorical groups (buckets), making analysis and visualization easier.**
