# 🧬 BioTech Lab Assistant | دستیار آزمایشگاه بیوتکنولوژی

[**GitHub Profile**](https://github.com/AlK9877)

---

## 🇬🇧 English Overview

**BioTech Lab Assistant** is a modern, responsive, client-side web application designed to accelerate routine biotechnology bench calculations and bioinformatics workflows. Built specifically for medical lab scientists, biotechnology researchers, students, and lab technicians to eliminate manual calculation errors, standardize protocols, and save critical benchwork time.

---

### ✨ Key Features & Modules

1. **PCR Master Mix Calculator:**
   - Single-reaction volume breakdown and bulk master mix volume scaling.
   - Dynamic compensation for pipetting loss via customizable excess margins (default: 10%).
   - Automatic balancing of Nuclease-free $\text{H}_2\text{O}$ and total bulk volume calculations.

2. **Western Blot ECL Substrate Calculator:**
   - Membrane surface area-based reagent volume estimation (Mini-gel: $7 \times 8\text{ cm}$, Midi-gel: $8 \times 10\text{ cm}$, or Custom dimensions).
   - Commercial kit ratio presets: Standard $1:1$ ratio (e.g., Pierce™ ECL, Bio-Rad Clarity) and $40:1$ ratio kits.
   - Calculates exact volumes for Luminol/Solution A and Peroxide/Solution B.

3. **Universal Dilution & Molarity Converter:**
   - $C_1V_1 = C_2V_2$ serial & stock dilution solver with flexible units ($\text{M, mM, µM, nM}$ and $\text{L, mL, µL}$).
   - Mass-to-Molarity converter: Computes required solute mass in grams ($g$) and milligrams ($mg$) based on target volume, concentration, and molecular weight.

4. **Sequence & GC Content Tool:**
   - Accepts raw nucleotide text and standard FASTA formats (DNA/RNA).
   - Real-time length, GC%, and AT% metrics.
   - **Primer Melting Temperature ($T_m$):** Computed via standard Marmur / Wallace-Itakura empirical rules.
   - **High-Precision ssDNA MW:** Accurate molecular weight estimation accounting for individual nucleotide weights and $5'$ monophosphate adjustment.
   - Interactive base counts ($A, T/U, C, G$), $5' \to 3'$ Reverse Complement generator, and Frame 1 protein translation.
   - One-click copy-to-clipboard buttons with live feedback.

5. **Multi-Format Lab Sheet Export:**
   - Instantly export comprehensive experimental records into **Word (.docx)**, **Excel (.xls)**, **CSV (.csv)**, and **Plain Text (.txt)** formats directly inside the browser using client-side JSZip.

6. **Trilingual & RTL Support:**
   - Seamless on-the-fly toggling between **English (EN)**, **فارسی (FA - RTL with Vazirmatn typography)**, and **Deutsch (DE)** without page reload.

---

### 🚀 Getting Started & Deployment

This application is built as a zero-dependency, single-file (`index.html`) web application ready for instant deployment on **GitHub Pages**:

1. Clone or download `index.html`.
2. Open `index.html` in any modern web browser (no local server or backend required).
3. To host on GitHub Pages:
   - Push `index.html` to your GitHub repository.
   - Navigate to **Settings** > **Pages** > Select branch `main` and root `/` > Click **Save**.

---

## 🇮🇷 معرفی به زبان فارسی

**دستیار آزمایشگاه بیوتکنولوژی (BioTech Lab Assistant)** یک وب‌اپلیکیشن سبک، واکنش‌گرا و سمت کلاینت است که برای سرعت‌بخشیدن و به حداقل رساندن خطاهای محاسباتی در آزمایشگاه‌های بیوتکنولوژی، تشخیص طبی، ژنتیک و بیولوژی مولکولی توسعه یافته است.

---

### ✨ قابلیت‌ها و ماژول‌های برنامه

۱. **محاسبه‌گر مستر میکس PCR:**
   - تفکیک اجزای واکنش برای ۱ چاهک و محاسبه حجم تجمیعی مستر میکس (Bulk Mix).
   - احتساب خطای پیپتینگ و اتلاف محلول با امکان تعیین درصد مازاد (پیش‌فرض ۱۰٪).
   - بالانس خودکار حجم آب عاری از نوکلئاز بر اساس حجم نهایی واکنش.

۲. **محاسبه‌گر سوبسترای وسترن بلات (ECL):**
   - تعیین حجم بهینه محلول کاری بر اساس سطح و ابعاد غشا (مینی‌ژل، مدی‌ژل یا ابعاد سفارشی به سانتی‌متر).
   - پشتیبانی از نسبت‌های استاندارد کیت‌های تجاری ($1:1$ و $40:1$).
   - تفکیک دقیق حجم معرف A (لومینول) و معرف B (پراکسید).

۳. **مبدل رقت و غلظت مولاری:**
   - حل سریع معادلات رقت‌سازی $C_1V_1 = C_2V_2$ با واحدهای متنوع غلظت و حجم.
   - محاسبه دقیق جرم ماده حل‌شونده بر حسب گرم و میلی‌گرم با دریافت وزن مولکولی (Molecular Weight).

۴. **آنالیز توالی ژنتیکی و درصد GC:**
   - پشتیبانی از توالی‌های خام و فرمت استاندارد FASTA (برای DNA و RNA).
   - محاسبه درصد GC و AT و شمارش تفکیکی بازهای نیتروژنی ($A, T/U, C, G$).
   - **محاسبه دمای ذوب پرایمر ($T_m$):** محاسبه بر اساس فرمول‌های استاندارد والاس و مارمور.
   - **تخمین دقیق وزن مولکولی (ssDNA):** محاسبه با لحاظ کردن جرم مولی دقیق تک‌تک نوکلئوتیدها و تصحیح پیوند فسفات.
   - تولید توالی مکمل معکوس ($5' \to 3'$) و ترجمه پروتئینی در فریم شماره ۱.
   - دکمه‌های کپی سریع در حافظه (Copy to Clipboard) با فیدبک بصری.

۵. **خروجی چندفرمته برگه کار آزمایشگاه (Lab Sheet):**
   - امکان دانلود خلاصه تمام محاسبات آزمایشگاهی در قالب فرمت‌های **Word (.docx)**، **Excel (.xls)**، **CSV** و **Text (.txt)** به‌صورت کاملاً آفلاین و درون مرورگر.

۶. **رابط کاربری ۳ زبانه:**
   - جابه‌جایی آنی میان زبان‌های **فارسی (راست‌به‌چپ با فونت زیبای وزیرمتن)**، **انگلیسی** و **آلمانی** بدون نیاز به بارگذاری مجدد صفحه.

---

## 👨‍🔬 About the Author / درباره توسعه‌دهنده

**English:**  
This project was designed and built after completing the **"Web App Design for Biotechnologists with AI"** course. It was developed with the goal of empowering laboratory colleagues, students, and life-science researchers with accessible, precise, and practical calculation tools at the bench.

**فارسی:**  
این پروژه پس از گذراندن دوره **«طراحی وب‌اپلیکیشن برای بایوتکنولوژیست‌ها به کمک هوش مصنوعی»** توسعه یافته است. هدف از ایجاد این ابزار، ارائه راهکاری دقیق، سریع و در دسترس برای کمک به همکاران آزمایشگاهی، محققان و فعالان علوم زیستی جهت پیشگیری از خطاهای انسانی در پیپتینگ و آماده‌سازی معرف‌ها بوده است.

* **GitHub Profile:** [@AlK9877](https://github.com/AlK9877)
