# Netflix Content Analysis Dashboard

**Data Analysis & Visualization | Tableau Public · Dashboard · Data Visualization**

โปรเจกต์วิเคราะห์ข้อมูลคอนเทนต์ของ Netflix และนำเสนอผลผ่าน Interactive Dashboard ด้วย Tableau โดยเน้นการสำรวจประเภทคอนเทนต์ ประเทศ แนวหนัง ระดับผู้ชม นักแสดง ผู้กำกับ และแนวโน้มการเพิ่มคอนเทนต์ในแต่ละช่วงเวลา

## Project Overview

โปรเจกต์นี้ใช้ข้อมูล Netflix Titles มาสร้าง Visualization และ Dashboard สำหรับดูภาพรวมของภาพยนตร์และรายการโทรทัศน์ในหลายมิติ

ข้อมูลถูกนำมาจัดกลุ่มและแสดงผลผ่านกราฟหลายรูปแบบ เช่น Map, Line Chart, Bar Chart และ Donut Chart เพื่อให้สามารถเปรียบเทียบจำนวนคอนเทนต์และดูแนวโน้มของข้อมูลได้ง่ายขึ้น

Dashboard แบ่งออกเป็น 2 หน้าหลัก ได้แก่ **Content Overview** และ **Content Analysis**

## Live Interactive Dashboard

สามารถทดลองใช้งาน Dashboard ผ่าน Tableau Public ได้ที่

[View Interactive Dashboard on Tableau Public](https://public.tableau.com/views/NetflixContentAnalysisDashboard_17871701191730/ContentAnalysis?:language=th-TH&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

## Data Fields Used

ตัวแปรหลักที่ใช้ในการสร้าง Visualization ได้แก่

- `show_id`
- `type`
- `title`
- `country`
- `date_added`
- `release_year`
- `rating`
- `duration`
- `director`
- `cast`
- `listed_in`

มีการใช้ข้อมูลเหล่านี้ในการจัดกลุ่ม นับจำนวน เปรียบเทียบ และสร้างกราฟใน Dashboard

## Dashboard Overview

### 1. Content Overview

หน้าแรกใช้สำหรับดูภาพรวมของข้อมูล Netflix โดยมีการวิเคราะห์หลัก เช่น

- จำนวนคอนเทนต์ตามประเทศ
- แนวโน้มจำนวนคอนเทนต์ที่เพิ่มเข้ามาตามปี
- การเปรียบเทียบ Movie และ TV Show
- การแบ่งระดับผู้ชมจาก Rating
- การดูแนวโน้มคอนเทนต์ที่เกี่ยวข้องกับประเทศไทย

<p align="center">
  <img src="screenshots/01-content-overview.png" width="850" alt="Netflix Content Overview Dashboard">
</p>

### Movie vs TV Show

จากข้อมูลใน Dashboard มีคอนเทนต์ทั้งหมด **6,232 รายการ**

แบ่งเป็น

- **Movie:** 4,263 รายการ
- **TV Show:** 1,969 รายการ

จากข้อมูลชุดนี้ Movie มีจำนวนมากกว่า TV Show อย่างเห็นได้ชัด

### Audience Level

นำข้อมูล Rating มาจัดกลุ่มเป็นระดับผู้ชม เช่น

- Adult
- Teen
- Family
- Kids
- Unsure

จากนั้นเปรียบเทียบจำนวนคอนเทนต์ในแต่ละระดับ โดยแยกระหว่าง Movie และ TV Show

### Content Trend

ใช้ Date Added เพื่อดูแนวโน้มของจำนวนคอนเทนต์ที่ถูกเพิ่มเข้าสู่ชุดข้อมูลในแต่ละปี และเปรียบเทียบแนวโน้มระหว่าง Movie กับ TV Show

## 2. Content Analysis

หน้าที่สองใช้สำหรับดูรายละเอียดของข้อมูลเพิ่มเติม เช่น ประเทศ แนวหนัง ผู้กำกับ และนักแสดง

<p align="center">
  <img src="screenshots/02-content-analysis.png" width="850" alt="Netflix Content Analysis Dashboard">
</p>

### Country Analysis

ใช้แผนที่สำหรับเปรียบเทียบข้อมูลคอนเทนต์ระหว่างประเทศ และเลือกประเทศตัวแทนจากแต่ละทวีปเพื่อช่วยให้เห็นความแตกต่างของข้อมูลในแต่ละพื้นที่

### Popular Content Categories

จากการจัดอันดับประเภทคอนเทนต์ พบหมวดหมู่ที่มีจำนวนรายการสูง เช่น

| Content Category | Number of Titles |
|---|---:|
| International Movies | 1,927 |
| Dramas | 1,623 |
| Comedies | 1,113 |
| International TV Shows | 1,001 |
| Documentaries | 668 |
| TV Dramas | 599 |
| Action & Adventure | 597 |
| Independent Movies | 552 |
| TV Comedies | 436 |
| Thrillers | 392 |

จาก Dashboard หมวด **International Movies** มีจำนวนรายการสูงที่สุดในข้อมูลที่นำมาวิเคราะห์

### Top Directors

สร้าง Bar Chart เพื่อดูผู้กำกับที่มีผลงานปรากฏในข้อมูล Netflix มากที่สุด

ตัวอย่างผู้กำกับที่อยู่ในอันดับต้น ได้แก่

- Jan Suter
- Raúl Campos
- Marcus Raboy

### Top Actors

สร้างการจัดอันดับนักแสดงจากจำนวนผลงานที่ปรากฏในข้อมูล

ตัวอย่างนักแสดงที่อยู่ในอันดับต้น ได้แก่

- Anupam Kher
- Shah Rukh Khan
- Om Puri

การวิเคราะห์ส่วนนี้เป็นการนับจำนวนรายการที่ชื่อของนักแสดงหรือผู้กำกับปรากฏใน Dataset ไม่ได้หมายถึงการจัดอันดับความนิยมจากจำนวนผู้ชม

## Analysis Areas

- Content Type Analysis
- Genre Analysis
- Country Analysis
- Audience Rating Analysis
- Actor Analysis
- Director Analysis
- Content Trend Analysis
- Movie vs TV Show Comparison

## Data Visualization

Visualization ที่ใช้ในโปรเจกต์ประกอบด้วย

- **Map** — แสดงและเปรียบเทียบข้อมูลตามประเทศ
- **Line Chart** — ดูแนวโน้มจำนวนคอนเทนต์ตามเวลา
- **Bar Chart** — เปรียบเทียบและจัดอันดับ Genre, Actor และ Director
- **Donut Chart** — เปรียบเทียบสัดส่วน Movie และ TV Show

## Key Findings

จาก Dashboard สามารถสังเกตได้ว่า

- Movie มีจำนวนมากกว่า TV Show ในข้อมูลที่นำมาวิเคราะห์
- International Movies เป็นหมวดหมู่ที่มีจำนวนคอนเทนต์มากที่สุด
- จำนวนคอนเทนต์ที่ถูกเพิ่มเข้าสู่ข้อมูลมีการเปลี่ยนแปลงอย่างเห็นได้ชัดตามช่วงเวลา
- ประเทศ แนวหนัง Rating นักแสดง และผู้กำกับสามารถนำมาใช้เพื่อดูความแตกต่างของคอนเทนต์ในหลายมิติ

ผลที่ได้จากโปรเจกต์นี้เน้นการสำรวจและสรุปข้อมูลจาก Dataset ผ่าน Visualization มากกว่าการสร้างแบบจำลองเพื่อพยากรณ์

## Skills Demonstrated

- Data Visualization
- Dashboard Design
- Exploratory Data Analysis
- Data Grouping
- Data Comparison
- Geographic Visualization
- Trend Analysis
- Interactive Dashboard Development
- Data Storytelling

## Tools & Technologies

- Tableau Public
- Tableau Desktop Public Edition

## Project Activities

โปรเจกต์นี้ครอบคลุมตั้งแต่การนำข้อมูลเข้าสู่ Tableau การสร้าง Worksheets สำหรับวิเคราะห์ข้อมูลในแต่ละมิติ การเลือกประเภทกราฟให้เหมาะกับข้อมูล การจัดองค์ประกอบ Dashboard และการ Publish ผลงานผ่าน Tableau Public

## Project Files

```text
netflix-content-analysis-tableau/
│
├── README.md
├── Netflix Content Analysis Dashboard.twbx
│
└── screenshots/
    ├── 01-content-overview.png
    └── 02-content-analysis.png
```

## Project Type

**Academic Project — Data Analysis & Interactive Dashboard Development**

โปรเจกต์นี้จัดทำขึ้นเพื่อฝึกการวิเคราะห์และนำเสนอข้อมูลด้วย Tableau ตั้งแต่การสร้าง Worksheets การเปรียบเทียบข้อมูลในหลายมิติ ไปจนถึงการรวม Visualization เป็น Interactive Dashboard

> **Note:** Repository นี้จัดทำขึ้นเพื่อการศึกษาและการนำเสนอผลงานใน Portfolio
