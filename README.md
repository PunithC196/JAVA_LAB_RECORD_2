# JAVA_LAB_RECORD_2

# LAB 2 - Object-Oriented Programming with Java (OOPS-JAVA)

**Student:** Punith C
**USN:** 1BF25CS196
**Date of execution:** 17-10-2026
**Tools used:** Notepad (source code), Command Prompt (`javac` and `java`)

---

## Files in this submission

| File | Description |
|---|---|
| `LAB-2-OOPS-JAVA.docx` | Lab record: for each program, the code screenshot, a simple explanation, the output screenshot and a verification |
| `LAB-2-OOPS-JAVA-Images.zip` | The 12 trimmed screenshots, numbered in document order |
| `README.md` | This file |

The Word document has the header "LAB 2" and the footer "Punith.C(1BF25CS196)" with page numbers on every page.

---

## Programs

| No. | File | What it does | Concepts |
|---|---|---|---|
| 1 | `Books.java` | Stores book details, searches by ID or title, finds the costlier book, counts books created | Class and objects, constructor, `this`, method overloading, static variable and method |
| 2 | `TypeCasting.java` | Splits an amount into integer and decimal parts | Scanner, explicit type casting |
| 3 | `ProductPrices.java` | Reads 10 prices; finds max, min, average and count above Rs. 1000 | Arrays, loops |
| 4 | `StudentDemo.java` | Accepts and displays USN and name of two students | Class and objects, passing Scanner to a method |
| 5 | `VehicleDemo.java` | Calculates the parking bill for three vehicles | Overloading, `static final`, private field with getter, static method |

---

## How to compile and run

Open Command Prompt, go to the folder that holds the `.java` files, and run:

```
cd C:\Users\admin\Desktop\1BF25CS196-OOPS-JAVA

javac Books.java
java Books

javac TypeCasting.java
java TypeCasting

javac ProductPrices.java
java ProductPrices

javac StudentDemo.java
java StudentDemo

javac VehicleDemo.java
java VehicleDemo
```

Inputs used in the screenshots:

| Program | Input typed |
|---|---|
| Books | none |
| TypeCasting | `1270.75` |
| ProductPrices | `500 1200 300 600 500 700 1140 3000 450 100` |
| StudentDemo | `1BF25CS196`, `Punith.C`, `1BF25CS656`, `Pallavi.C` (one per line) |
| VehicleDemo | none |

---

## Results (checked by hand)

| Program | Result |
|---|---|
| Books | ID 102 found, title "Data Structures" found, costlier book is Book 103 (Rs. 660), total books = 3 |
| TypeCasting | Integer part 1270, decimal part 0.75 |
| ProductPrices | Max 3000.0, min 100.0, average 849.0, 3 products above Rs. 1000 |
| StudentDemo | Both students stored and displayed correctly |
| VehicleDemo | Two-wheeler Rs. 60, Car Rs. 160, Bus Rs. 120 (charge = 20 x multiplier x hours) |

---

## Image list (all taken on 17-10-2026)

| Image | Time |
|---|---|
| `01_Books_Code_Part1_Book-Class.png` | 08:34:28 |
| `02_Books_Code_Part2_Books-Main.png` | 08:34:39 |
| `03_Books_Output.png` | 08:33:50 |
| `04_TypeCasting_Code.png` | 09:10:37 |
| `05_TypeCasting_Output.png` | 09:11:28 |
| `06_ProductPrices_Code.png` | 09:10:46 |
| `07_ProductPrices_Output.png` | 09:11:28 |
| `08_StudentDemo_Code.png` | 09:10:55 |
| `09_StudentDemo_Output.png` | 09:11:28 |
| `10_VehicleDemo_Code_Part1_Vehicle-Class.png` | 09:11:05 |
| `11_VehicleDemo_Code_Part2_VehicleDemo-Main.png` | 09:11:05 |
| `12_VehicleDemo_Output.png` | 09:12:16 |

Each image ends with a strip cut from the original screenshot's taskbar clock, so the time and date are visible in the image itself.

---

## Notes

- **Rupee sign shows as `?` in the Books output.** The code prints the rupee symbol, but the Windows Command Prompt cannot display it. To see it correctly, run `chcp 65001` and then `java -Dstdout.encoding=UTF-8 Books`. Or print `Rs.` instead of the symbol.
- **Decimal values in TypeCasting.** Some inputs (for example `1270.7`) can print a tiny extra fraction such as `0.7000000000000455`, because `double` stores decimals in binary.
- Books and VehicleDemo code were split into two images (the class, then the main method) so the text stays readable in the document.
