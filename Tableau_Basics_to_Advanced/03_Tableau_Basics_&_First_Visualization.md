# 📂 Dataset Used

## 🎮 Video Game Sales Dataset

Is Tableau project me hum **Video Game Sales Dataset** ka use karenge jo ki Humne Kaggle se Liya hai.

Ye dataset duniya bhar me **16,500+ video games** ki sales information provide karta hai. Iski help se hum different charts, dashboards aur insights create karna seekhenge.

Ye Dataset CSV me hai 
---

# 📌 About the Dataset

Is dataset me un video games ki information di gayi hai jinki sales **100,000 copies (1 lakh copies)** se zyada hui hain.

Dataset me total **16,598 records** hain aur isme alag-alag games ki sales, platform, genre, publisher aur worldwide sales ki details available hain.

---

# 📊 Dataset Columns

| Column Name | Description |
|-------------|-------------|
| **Rank** | Overall sales ke basis par game ki ranking |
| **Name** | Video Game ka naam |
| **Platform** | Game kis platform ke liye launch hua (PC, PS4, Xbox, etc.) |
| **Year** | Game release hone ka year |
| **Genre** | Game kis category ka hai (Action, Sports, Racing, etc.) |
| **Publisher** | Game publish karne wali company |
| **NA_Sales** | North America me sales (Millions me) |
| **EU_Sales** | Europe me sales (Millions me) |
| **JP_Sales** | Japan me sales (Millions me) |
| **Other_Sales** | Baaki countries ki sales (Millions me) |
| **Global_Sales** | Puri duniya ki total sales (Millions me) |

---

# 💡 Is Dataset Se Hum Kya Analyze Kar Sakte Hain?

- 🎮 Top Selling Games
- 🏆 Top Publishers
- 🎯 Most Popular Game Genres
- 💻 Platform-wise Sales
- 🌍 Region-wise Sales (NA, EU, JP, Other)
- 📅 Year-wise Game Releases
- 🌎 Global Sales Analysis

---

# 🎯 Why We Selected This Dataset?

Humne ye dataset choose kiya kyunki:

- ✅ Dataset clean aur beginner-friendly hai.
- ✅ Visualization ke liye perfect hai.
- ✅ Multiple charts aur dashboards bana sakte hain.
- ✅ Real-world business analysis practice karne ke liye useful hai.
- ✅ Tableau ke almost saare basic concepts is dataset se cover ho jate hain.

---

# 📌 Quick Summary

- **Dataset Name:** Video Game Sales
- **Total Records:** 16,598
- **Main Topic:** Video Game Sales Analysis
- **Purpose:** Data Visualization & Dashboard Creation in Tableau

> 💡 **Note:** Is dataset ka use hum Tableau me different charts, graphs aur interactive dashboards banane aur data analysis seekhne ke liye karenge.




# 📊 Tableau Basics & First Visualization

## 📥 Importing a Dataset in Tableau

Tableau open karne ke baad **Connect** section dikhai deta hai. Yahan se hum apna dataset import karte hain.

### Tableau Supported File Formats

Tableau kai tarah ki files ko support karta hai, jaise:

- Microsoft Excel (.xlsx)
- Text File (.csv, .txt)
- JSON File (.json)
- Microsoft Access
- PDF
- SQL Databases
- Google Sheets
- Web Data Connector

> Humara dataset **CSV (Comma Separated Values)** format me tha, isliye humne **Text File** option select kiya.

### Steps to Import CSV File

1. Tableau open karein.
2. **Connect** section me **Text File** select karein.
3. Apni CSV file browse karke open karein.
4. Tableau dataset ka preview dikhayega.
5. Neeche **Sheet 1 (Go to Worksheet)** par click karein.

Ab hum visualization (Charts, Graphs, Tables, Dashboard) banana shuru kar sakte hain.

---

# 📄 Tableau Worksheet Interface

Worksheet Tableau ka main working area hota hai jahan hum Drag & Drop karke visualizations create karte hain.

---

## 🧩 1. Data Pane

Left side me Data Pane hota hai jahan dataset ke saare fields dikhte hain.

Ye mainly do parts me divide hota hai:

### 📌 Dimensions

Dimensions categorical (Text) data hote hain.

**Example**

- Genre
- Name
- Platform
- Publisher
- Year

**Use**

- Data ko categorize karna
- Grouping karna
- Labels banana

---

### 📌 Measures

Measures numerical data hote hain.

**Example**

- Global Sales
- NA Sales
- EU Sales
- JP Sales
- Other Sales
- Rank

**Use**

- Calculations
- Charts
- Analysis
- Aggregation (SUM, AVG, COUNT etc.)

---

## 📌 Measure Names

Measure Names Tableau ka automatically generated field hai.

Ye dataset ke saare numerical columns ke **naam** store karta hai.

Example

- Global Sales
- EU Sales
- JP Sales
- Other Sales

---

## 📌 Measure Values

Measure Values Tableau ka automatically generated field hai.

Ye Measures ki **actual values** ko represent karta hai.

### Example

| Game | Global Sales | NA Sales | EU Sales |
|------|-------------:|----------:|----------:|
| GTA V | 25 | 10 | 8 |

Yahan

- Measure Names → Global Sales, NA Sales, EU Sales
- Measure Values → 25, 10, 8

### Use

Jab ek hi chart me multiple measures compare karne hote hain.

---

## 📄 2. Pages Shelf

Visualization ko page-wise ya value-wise dekhne ke liye use hota hai.

**Example**

Year ko Pages me drag karne par har year alag page me dikhega.

---

## 🎯 3. Filters Shelf

Sirf required data dikhane ke liye use hota hai.

**Example**

- Sirf Action Genre
- Sirf 2020 ka data

---

## 🎨 4. Marks Card

Visualization ki appearance control karta hai.

Options

- 🎨 Color → Color change karna
- 📏 Size → Size badhana ya ghataana
- 📝 Label → Data labels dikhana
- 🔍 Detail → Extra information add karna
- 💬 Tooltip → Hover information

---

## 📈 5. Columns Shelf

Yahan drag kiya gaya field **Horizontal (X-Axis)** ban jata hai.

Example

Year → Columns

---

## 📉 6. Rows Shelf

Yahan drag kiya gaya field **Vertical (Y-Axis)** ban jata hai.

Example

Global Sales → Rows

---

## 🖥️ 7. Visualization Area (Canvas)

Ye worksheet ka main area hota hai.

Yahin par charts aur graphs create hote hain.

---

## 📊 8. Show Me Panel

Right side me Show Me panel hota hai.

Ye selected fields ke according automatically suitable chart suggest karta hai.

**Note**

Show Me tabhi active hota hai jab hum kisi field ko worksheet me drag & drop karte hain.

Available Charts

- Bar Chart
- Line Chart
- Pie Chart
- Scatter Plot
- Tree Map
- Heat Map
- Histogram
- Bubble Chart
- Maps

---

# 📌 Quick Revision

| Component | Purpose |
|-----------|---------|
| Data Pane | Dataset ke fields |
| Dimensions | Categories/Text Data |
| Measures | Numerical Data |
| Measure Names | Measures ke naam |
| Measure Values | Measures ki values |
| Pages | Page-wise visualization |
| Filters | Data filtering |
| Marks Card | Chart formatting |
| Columns | X-Axis |
| Rows | Y-Axis |
| Canvas | Visualization area |
| Show Me | Chart suggestions |
