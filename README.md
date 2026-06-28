# ☀️ Design of Standalone PV System — تصميم نظام طاقة شمسية معزول

> **Zagazig University — Faculty of Engineering | Level 200**
> 
> **Omar Mohamed Abd El-Hamid Ibrahim & Marwan Mostafa Ahmed El-Saei**

---

## 🇬🇧 English

### Project Overview

This project presents the **design and simulation of a standalone (off-grid) photovoltaic system** using **PVsyst V7.4.8**. The system is designed for **Dakar, Senegal** — a location with strong and consistent solar radiation throughout the year — making it an ideal case study for off-grid electricity generation.

The system is sized to meet residential load demands independently, without any connection to the utility grid.

---

### ⚙️ System Specifications

| Parameter | Value |
|-----------|-------|
| **Software** | PVsyst V7.4.8 |
| **System Type** | Standalone (Off-Grid) with Batteries |
| **Location** | Dakar/Taklou, Senegal |
| **Latitude / Longitude** | 14.74°N / -17.48°W |
| **Altitude** | 20 m |
| **Time Zone** | UTC-1 |
| **Tilt Angle** | 15° |
| **Azimuth** | 0° (South-facing) |

---

### 🔋 System Components

#### PV Array
| Parameter | Value |
|-----------|-------|
| Module Type | Generic Poly 60 Wp, 36 cells |
| Number of Modules | 8 units (4 strings × 2 in series) |
| Nominal Power (STC) | **480 Wp** |
| Module Area | 4.5 m² |
| Operating Power (50°C) | 432 Wp |

#### Battery Storage
| Parameter | Value |
|-----------|-------|
| Technology | Lead-acid, Sealed Gel |
| Number of Units | 4 (2 parallel × 2 series) |
| Voltage | 24 V |
| Nominal Capacity | **320 Ah (C10)** |
| Stored Energy | 6.1 kWh |
| Min. Discharge SOC | 20% |

#### Controller
| Parameter | Value |
|-----------|-------|
| Type | Universal MPPT Charge Controller |
| Max/EURO Efficiency | 97.0 / 95.0% |
| Temp. Coefficient | -5.0 mV/°C/Element |

---

### 🏠 Load Profile

Daily residential consumption with **seasonal modulation**:

| Season | Total Daily Energy |
|--------|--------------------|
| Summer (Jun–Aug) | 2,009 Wh/day |
| Autumn (Sep–Nov) | 2,343 Wh/day |
| Winter (Dec–Feb) | 2,553 Wh/day |
| Spring (Mar–May) | 2,343 Wh/day |
| **Annual Average** | **2.3 kWh/day** |

**Appliances included:** Lamps (LED), TV/PC/Mobile, Domestic appliances, Fridge/Deep-freeze, Dish & Cloth washer, Stand-by consumers.

---

### 📊 Simulation Results

#### Annual Energy Balance

| Metric | Value |
|--------|-------|
| Available Solar Energy | **810.52 kWh/year** |
| Useful Energy Supplied to User | **784.05 kWh/year** |
| Excess (Unused) Energy | 10.99 kWh/year |
| Missing Energy | 59.39 kWh/year |
| **Performance Ratio (PR)** | **74.89%** |
| **Solar Fraction (SF)** | **92.96%** |
| Specific Production | 1,633 kWh/kWp/year |

#### Monthly Solar Fraction

| Month | Solar Fraction |
|-------|---------------|
| January | 88.0% |
| February | 96.3% |
| March | 98.4% |
| April | **100%** |
| May | **100%** |
| June | **100%** |
| July | **100%** |
| August | 92.2% |
| September | 86.4% |
| October | 91.0% |
| November | 89.2% |
| December | 77.8% |

#### Key System Losses

| Loss Type | Fraction |
|-----------|----------|
| PV temperature loss | -11.61% |
| Ohmic wiring loss | -3.53% |
| Module quality loss | -2.50% |
| Converter loss | -4.00% |
| Battery efficiency loss | -0.93% |

---

### ✅ Conclusion

The designed standalone PV system demonstrated strong performance under Dakar's solar conditions:
- The system achieves full solar coverage (SF = 100%) during **4 months** of the year (April–July).
- Overall annual solar fraction of **92.96%**, meaning the system reliably covers most of the residential energy demand.
- Performance Ratio of **74.89%** reflects a well-optimized system design.
- The system is a **practical and cost-effective** off-grid electricity solution for locations with high solar irradiation.

---


### 🛠️ Tools Used

- **PVsyst V7.4.8** — Photovoltaic system simulation software
- **MeteoNorm 7.2** — Weather data source (Dakar/Yoff station, synthetic)

---

---

## 🇪🇬 العربي

### نظرة عامة على المشروع

يقدم هذا المشروع **تصميم ومحاكاة نظام طاقة شمسية معزول (Off-Grid)** باستخدام برنامج **PVsyst V7.4.8**. تم تصميم النظام لمنطقة **داكار، السنغال** — وهي منطقة تتمتع بإشعاع شمسي قوي ومستمر على مدار العام — مما يجعلها نموذجًا مثاليًا لاختبار فاعلية الأنظمة الشمسية المعزولة.

النظام مُصمَّم لتلبية احتياجات أحمال سكنية بشكل مستقل، دون أي اتصال بشبكة الكهرباء العامة.

---

### ⚙️ المواصفات التقنية للنظام

| المعامل | القيمة |
|---------|--------|
| **البرنامج المستخدم** | PVsyst V7.4.8 |
| **نوع النظام** | معزول (Off-Grid) مع بطاريات |
| **الموقع** | داكار/تاكلو، السنغال |
| **خط العرض / الطول** | 14.74°N / 17.48°W- |
| **الارتفاع** | 20 م |
| **زاوية الميل** | 15° |
| **الزاوية الأزيموتية** | 0° (متجه نحو الجنوب) |

---

### 🔋 مكونات النظام

#### الألواح الشمسية (PV Array)
| المعامل | القيمة |
|---------|--------|
| نوع الوحدة | Generic Poly 60 Wp, 36 خلية |
| عدد الوحدات | 8 وحدات (4 سلاسل × 2 على التوالي) |
| القدرة الاسمية (STC) | **480 Wp** |
| مساحة الألواح | 4.5 م² |

#### البطاريات
| المعامل | القيمة |
|---------|--------|
| التقنية | رصاص-حمض، Sealed Gel |
| عدد الوحدات | 4 وحدات (2 موازي × 2 على التوالي) |
| الجهد | 24 فولت |
| السعة الاسمية | **320 Ah** |
| الطاقة المخزنة | 6.1 kWh |

#### وحدة التحكم
- **نوع:** Universal MPPT Charge Controller
- **الكفاءة القصوى:** 97.0%

---

### 🏠 الأحمال الكهربائية

استهلاك سكني يومي مع **تعديل موسمي**:

| الفصل | إجمالي الطاقة اليومية |
|-------|-----------------------|
| الصيف (يونيو–أغسطس) | 2,009 وات.ساعة/يوم |
| الخريف (سبتمبر–نوفمبر) | 2,343 وات.ساعة/يوم |
| الشتاء (ديسمبر–فبراير) | 2,553 وات.ساعة/يوم |
| الربيع (مارس–مايو) | 2,343 وات.ساعة/يوم |
| **المتوسط السنوي** | **2.3 كيلوواط.ساعة/يوم** |

**الأجهزة المشمولة:** إضاءة LED، تلفزيون/كمبيوتر/موبايل، أجهزة منزلية، ثلاجة، غسالة، أحمال وضع الاستعداد.

---

### 📊 نتائج المحاكاة

#### الميزان الطاقوي السنوي

| المؤشر | القيمة |
|--------|--------|
| الطاقة الشمسية المتاحة | **810.52 كيلوواط.ساعة/سنة** |
| الطاقة المُورَّدة للمستخدم | **784.05 كيلوواط.ساعة/سنة** |
| الطاقة الفائضة (غير مستخدمة) | 10.99 كيلوواط.ساعة/سنة |
| الطاقة المفقودة (عجز) | 59.39 كيلوواط.ساعة/سنة |
| **نسبة الأداء (PR)** | **74.89%** |
| **الكسر الشمسي (SF)** | **92.96%** |
| الإنتاج النوعي | 1,633 كيلوواط.ساعة/كيلوواط.ذروة/سنة |

---

### ✅ الخلاصة

أثبت النظام المُصمَّم أداءً قويًا في ظروف داكار الشمسية:
- يحقق النظام تغطية شمسية كاملة (SF = 100%) خلال **4 أشهر** في السنة (أبريل–يوليو).
- الكسر الشمسي السنوي **92.96%** يعني أن النظام يغطي الغالبية العظمى من احتياجات الطاقة السكنية.
- نسبة الأداء **74.89%** تعكس تصميمًا محسَّنًا وفعَّالًا.
- النظام يُعدُّ **حلًا عمليًا وفعَّالًا من حيث التكلفة** لتوليد الكهرباء بعيدًا عن الشبكة.

---
*Simulated with PVsyst V7.4.8 | Weather data: MeteoNorm 7.2 (Dakar/Yoff, Synthetic)*
