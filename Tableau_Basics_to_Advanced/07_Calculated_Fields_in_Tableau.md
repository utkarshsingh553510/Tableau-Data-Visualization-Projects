# 🧮 Calculated Fields in Tableau

## 📌 What is a Calculated Field?

**Calculated Field** Tableau ka ek feature hai jisme hum formulas likhkar **naya column (field)** create kar sakte hain.

Simple words me:

> **Calculated Field ka use existing columns ki help se naye values ya calculations create karne ke liye kiya jata hai.**

Ye bilkul Excel ke Formula aur SQL ke Calculated Column ki tarah kaam karta hai.

---

# 💡 Real-Life Example

Maan lo ek Student dataset hai.

| Name | Math | Science |
|------|------:|---------:|
| Rahul | 80 | 90 |

Agar hume Total Marks chahiye to dataset me Total column nahi hai.

Hum Calculated Field bana sakte hain.

```
Math + Science
```

Output

```
170
```

---

# 🎮 Example: Video Game Sales Dataset

Humare dataset me ye columns hain:

- Global Sales
- EU Sales
- NA Sales
- JP Sales
- Other Sales

Ab maan lo hume Global Sales aur EU Sales ka difference nikalna hai.

Dataset me aisa koi column nahi hai.

To hum Calculated Field create karenge.

---

# 🛠️ How to Create a Calculated Field

### Step 1

Data Pane me Right Click karein.

### Step 2

** koi bhi column select kro let say Global Sales -> Create → Calculated Field** select karein.

let say hume ye calculate krna hai Global Sales - EU Sales to sbse pahele Global Sales pr click kro and Create -> calculated field 

### Step 3

Field ka naam dein. 
Example

```
Global Sales - EU Sales
```

### Step 4

Formula likhein.

```text
[Global Sales] - [EU Sales]
```

### Step 5

OK par click karein.

---

## Output

Data Pane me ek naya field create ho jayega.

```
Global Sales - EU Sales
```

Ab is field ko kisi bhi chart me use kar sakte hain.

---

# 📊 Example 2: Percentage of Global Sales

Ek aur Calculated Field banate hain.

### Field Name

```
Percentage of Global Sales
```

### Formula

```text
([EU Sales] / [Global Sales]) * 100
```

Is formula se pata chalega ki Global Sales me se kitna percentage sirf Europe se aaya.

---

## Output

Data Pane me ek aur naya field create ho jayega.

```
Percentage of Global Sales
```

Ab is field ko Bar Chart, Pie Chart ya Table me use kar sakte hain.

---

# 📈 Visualization

Screenshot me:

- **Year (Bin)** → Columns
- **SUM(Global Sales - EU Sales)** → Rows
- **Genre** → Color

Is visualization se hum dekh sakte hain ki har **5-Year Group** me Global Sales aur EU Sales ke beech kitna difference tha aur kis Genre ka contribution sabse zyada tha.

---

# 🎯 Advantages of Calculated Fields

✅ Naye columns create kar sakte hain.

✅ Existing data par calculations kar sakte hain.

✅ Custom metrics bana sakte hain.

✅ Business analysis easy ho jata hai.

---

# 📌 Common Calculated Field Examples

### 1. Difference

```text
[Global Sales] - [EU Sales]
```

---

### 2. Addition

```text
[NA Sales] + [EU Sales]
```

---

### 3. Average

```text
([NA Sales] + [EU Sales]) / 2
```

---

### 4. Percentage

```text
([EU Sales] / [Global Sales]) * 100
```

---

### 5. Profit

```text
[Sales] - [Cost]
```

---

### 6. IF Condition

```text
IF [Global Sales] > 50 THEN
"High Sales"
ELSE
"Low Sales"
END
```

---

# 📊 Difference Between Bins and Calculated Fields

| Bins | Calculated Fields |
|------|-------------------|
| Numerical data ko groups me divide karta hai. | Formula use karke naya field create karta hai. |
| Grouping ke liye use hota hai. | Calculation ke liye use hota hai. |
| Example: Year (Bin) | Example: Global Sales - EU Sales |

---

# 📝 Summary

| Concept | Description |
|---------|-------------|
| Calculated Field | Formula se naya field create karna |
| Formula | Existing columns ka use karta hai |
| Output | Naya calculated column |
| Use | Analysis, Dashboard, Charts, Reports |

---

## 💡 Interview Point

> **Calculated Field is used to create a new field by applying formulas on existing fields. It helps perform custom calculations and build meaningful business metrics without modifying the original dataset.**
