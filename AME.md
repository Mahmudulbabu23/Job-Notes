# 🎯 সহকারী মেইন্টেন্যান্স ইঞ্জিনিয়ার (কম্পিউটার সায়েন্স)
## বাংলাদেশ মন্ত্রণালয় / ব্যাংক পরীক্ষা — সম্পূর্ণ পূর্ণাঙ্গ প্রিপারেশন গাইড
### ✍️ প্রতিটি টপিক সম্পূর্ণ বিস্তারিতভাবে আলোচিত

---

> **📌 শিক্ষকের কথা:** এই গাইডটি তৈরি করা হয়েছে বাংলাদেশ ব্যাংক ও বিভিন্ন মন্ত্রণালয়ের AME (CS) পরীক্ষার সিলেবাস বিশ্লেষণ করে। প্রতিটি টপিক এমনভাবে ব্যাখ্যা করা হয়েছে যেন পরীক্ষার হলে MCQ এবং লিখিত দুটোতেই সর্বোচ্চ নম্বর পাওয়া যায়। শুধু মুখস্থ না করে — **বুঝে পড়ো।**

---

## 📊 পরীক্ষার মানবণ্টন (সম্পূর্ণ)

| পরীক্ষার ধরন | বিষয় | নম্বর | সময় |
|---|---|---|---|
| MCQ | সাবজেক্ট রিলেটেড (CS) | ৭৫ | ১ ঘণ্টা |
| MCQ | গণিত | ১৫ | (একসাথে) |
| MCQ | সাধারণ জ্ঞান | ১০ | (একসাথে) |
| **MCQ মোট** | | **১০০** | **১ ঘণ্টা** |
| লিখিত | সাবজেক্ট রিলেটেড (CS) | ১৫০ | ২ ঘণ্টা |
| লিখিত | গণিত | ২০ | (একসাথে) |
| লিখিত | ইংরেজি | ৩০ | (একসাথে) |
| **লিখিত মোট** | | **২০০** | **২ ঘণ্টা** |
| **সর্বমোট** | | **৩০০** | **৩ ঘণ্টা** |

---

## 🔥 প্রশ্নের ওজন অনুযায়ী অধ্যয়নের অগ্রাধিকার

| অগ্রাধিকার | বিষয় | প্রশ্নের আনুমানিক হার |
|---|---|---|
| 🔴 সর্বোচ্চ | কম্পিউটার নেটওয়ার্কিং | ~২২% |
| 🔴 সর্বোচ্চ | DBMS | ~২০% |
| 🔴 সর্বোচ্চ | কম্পিউটার আর্কিটেকচার | ~২০% |
| 🔴 সর্বোচ্চ | প্রোগ্রামিং / OOP | ~১৮% |
| 🟡 মাঝারি | অপারেটিং সিস্টেম | ~১৫% |
| 🟡 মাঝারি | ডেটা স্ট্রাকচার ও অ্যালগরিদম | ~১২% |
| 🟡 মাঝারি | সাইবার সিকিউরিটি | ~১০% |
| 🟢 সহায়ক | গণিত | ১৫ (MCQ) + ২০ (লিখিত) |
| 🟢 সহায়ক | সাধারণ জ্ঞান | ১০ (MCQ) |

---

---

# ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
# অধ্যায় ১: কম্পিউটার আর্কিটেকচার ও হার্ডওয়ার
### 🔴 সর্বোচ্চ গুরুত্ব (~২০%)
# ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

---

## ১.১ CPU (Central Processing Unit) — বিস্তারিত

CPU হলো কম্পিউটারের **মস্তিষ্ক (Brain)**। এটি সমস্ত গাণিতিক হিসাব-নিকাশ এবং লজিক্যাল সিদ্ধান্ত গ্রহণ করে। CPU ছাড়া কম্পিউটার কোনো কাজই করতে পারে না।

### 🔷 CPU-এর তিনটি প্রধান অংশ:

#### ১. ALU — Arithmetic Logic Unit
- **কাজ:** দুই ধরনের অপারেশন করে —
  - **Arithmetic (গাণিতিক):** যোগ (+), বিয়োগ (−), গুণ (×), ভাগ (÷)
  - **Logical (লজিক্যাল):** AND, OR, NOT, XOR, comparison (>, <, =)
- **গুরুত্ব:** প্রতিটি প্রোগ্রামের প্রতিটি গণনা ALU-তে হয়। এটিই CPU-এর হৃদয়।
- **উদাহরণ:** `2 + 3 = 5` এই হিসাবটি ALU করে; `যদি A > B` এই তুলনাটিও ALU করে।

#### ২. CU — Control Unit
- **কাজ:** CPU-এর সমস্ত কার্যক্রম পরিচালনা ও সমন্বয় করে।
  - মেমোরি থেকে নির্দেশনা **Fetch (আনা)** করে
  - নির্দেশনা **Decode (বোঝা)** করে
  - ALU ও রেজিস্টারকে কাজের নির্দেশ দেয়
  - ডেটা ট্রান্সফার নিয়ন্ত্রণ করে
- **উপমা:** CU হলো কারখানার ম্যানেজারের মতো — সে নিজে কাজ করে না, কিন্তু সবাইকে নির্দেশ দেয়।

#### ৩. Register (রেজিস্টার)
CPU-এর ভেতরে অবস্থিত **অতি ক্ষুদ্র ও অতি দ্রুত** অস্থায়ী মেমোরি। এগুলো সরাসরি CPU সার্কিটের অংশ।

| রেজিস্টার | পূর্ণনাম | কাজ |
|---|---|---|
| **PC** | Program Counter | পরবর্তী নির্দেশনার মেমোরি ঠিকানা ধরে রাখে |
| **IR** | Instruction Register | বর্তমানে যে নির্দেশনা চলছে সেটি সংরক্ষণ করে |
| **MAR** | Memory Address Register | মেমোরিতে কোন ঠিকানায় যেতে হবে তা ধরে রাখে |
| **MDR** | Memory Data Register | মেমোরি থেকে আনা/পাঠানো ডেটা সাময়িক রাখে |
| **ACC** | Accumulator | ALU-এর হিসাবের ফলাফল সাময়িক রাখে |
| **SP** | Stack Pointer | Stack-এর উপরের অবস্থান নির্দেশ করে |

---

### 🔷 CPU-এর কাজের চক্র — Fetch-Decode-Execute Cycle

CPU প্রতিটি নির্দেশনা তিনটি ধাপে সম্পন্ন করে:

```
┌─────────────┐     ┌─────────────┐     ┌─────────────┐
│   FETCH     │────▶│   DECODE    │────▶│   EXECUTE   │
│ মেমোরি থেকে │     │ নির্দেশনা  │     │  ALU-তে     │
│ নির্দেশনা  │     │ বোঝা       │     │  কাজ করা   │
│ আনা         │     │             │     │             │
└─────────────┘     └─────────────┘     └─────────────┘
        ▲                                       │
        └───────────────────────────────────────┘
                    পরবর্তী চক্র শুরু
```

---

### 🔷 CPU Pipeline — ৫ ধাপের পাইপলাইন

পাইপলাইন হলো এমন একটি কৌশল যেখানে একসাথে একাধিক নির্দেশনার বিভিন্ন ধাপ একই সময়ে চলতে পারে, ঠিক যেমন একটি কারখানার অ্যাসেম্বলি লাইন।

```
IF → ID → EX → MEM → WB
```

| ধাপ | নাম | কাজ |
|---|---|---|
| **IF** | Instruction Fetch | Program Counter ব্যবহার করে মেমোরি থেকে নির্দেশনা আনা |
| **ID** | Instruction Decode | নির্দেশনা ডিকোড করা, রেজিস্টার পড়া |
| **EX** | Execute | ALU-তে গাণিতিক বা লজিক্যাল অপারেশন সম্পাদন |
| **MEM** | Memory Access | প্রয়োজনে মেমোরি থেকে ডেটা পড়া বা লেখা |
| **WB** | Write Back | ফলাফল রেজিস্টারে লেখা |

**পাইপলাইনের সুবিধা:** একই সময়ে ৫টি নির্দেশনার ৫টি ভিন্ন ধাপ চলতে পারে → CPU অনেক দ্রুত কাজ করে।

**পাইপলাইন Hazard (সমস্যা):**
- **Data Hazard:** পরবর্তী নির্দেশনা আগের ফলাফলের উপর নির্ভরশীল
- **Control Hazard:** Branch/Jump নির্দেশনায় পাইপলাইন ভেঙে যায়
- **Structural Hazard:** একই হার্ডওয়ার একসাথে দুটি কাজ করতে পারে না

---

### 🔷 RISC vs CISC — বিস্তারিত তুলনা

| বৈশিষ্ট্য | RISC (Reduced Instruction Set Computer) | CISC (Complex Instruction Set Computer) |
|---|---|---|
| **নির্দেশনার সংখ্যা** | কম (সাধারণত ৩২-১২৮টি) | বেশি (কয়েকশত) |
| **নির্দেশনার জটিলতা** | সহজ, সরল | জটিল, বহুমুখী |
| **গতি** | বেশি দ্রুত | তুলনামূলক ধীর |
| **নির্দেশনার আকার** | নির্দিষ্ট (Fixed) | পরিবর্তনশীল (Variable) |
| **Clock Cycle/নির্দেশনা** | সাধারণত ১ | একাধিক |
| **পাইপলাইন** | সহজ | কঠিন |
| **রেজিস্টার সংখ্যা** | বেশি | কম |
| **মেমোরি অ্যাক্সেস** | Load/Store নির্দেশনা দিয়েই | যেকোনো নির্দেশনায় |
| **বিদ্যুৎ খরচ** | কম | বেশি |
| **ব্যবহার** | স্মার্টফোন, ট্যাবলেট, এমবেডেড | Desktop PC, Server |
| **উদাহরণ** | ARM, MIPS, PowerPC | Intel x86, AMD x64 |

> 📌 **পরীক্ষায় বারবার আসে:** স্মার্টফোনে RISC আর্কিটেকচার ব্যবহার হয় কারণ এটি কম বিদ্যুৎ খরচ করে এবং তাপ কম উৎপন্ন করে।

---

## ১.২ মেমোরি হায়ারার্কি — সম্পূর্ণ বিবরণ

কম্পিউটারের মেমোরি বিভিন্ন স্তরে সাজানো থাকে। উপরের স্তর যত দ্রুত, দাম তত বেশি, আকার তত ছোট।

```
         ┌──────────────────┐  ← সবচেয়ে দ্রুত, সবচেয়ে ছোট, সবচেয়ে দামি
         │    Registers     │    (CPU-এর ভেতরে, Bytes পরিমাণ)
         └────────┬─────────┘
                  │
         ┌────────▼─────────┐
         │  Cache Memory    │    (L1: CPU-এ, L2: CPU-এর কাছে, L3: শেয়ারড)
         │   L1 → L2 → L3  │    (KB থেকে MB পরিমাণ)
         └────────┬─────────┘
                  │
         ┌────────▼─────────┐
         │   Main Memory    │    (RAM — Primary Memory)
         │      (RAM)       │    (GB পরিমাণ, উদ্বায়ী)
         └────────┬─────────┘
                  │
         ┌────────▼─────────┐
         │Secondary Memory  │    (HDD, SSD — Non-volatile)
         │   (HDD / SSD)    │    (TB পরিমাণ)
         └────────┬─────────┘
                  │
         ┌────────▼─────────┐
         │  Tertiary/Backup │    (Optical Disk, Tape, Cloud)
         │  (CD/DVD/Tape)   │    (সবচেয়ে ধীর, সবচেয়ে বড়)
         └──────────────────┘
```

---

### 🔷 Cache Memory — বিস্তারিত

Cache হলো CPU ও RAM-এর মাঝে একটি দ্রুতগতির মধ্যবর্তী মেমোরি। CPU যখন কোনো ডেটা দরকার হয়, প্রথমে Cache-এ খোঁজে।

| Cache | অবস্থান | আকার | গতি | কাজ |
|---|---|---|---|---|
| **L1 Cache** | CPU Chip-এর ভেতরে | 32–64 KB | অতি দ্রুত (1-4 cycle) | প্রতিটি CPU Core-এর নিজস্ব |
| **L2 Cache** | CPU Chip-এ বা কাছে | 256 KB – 4 MB | দ্রুত (4-12 cycle) | একটি বা কয়েকটি Core শেয়ার করে |
| **L3 Cache** | CPU Chip-এ | 4 MB – 64 MB | মোটামুটি দ্রুত | সব Core শেয়ার করে |

**Cache Hit:** CPU যা খুঁজছে তা Cache-এ পাওয়া গেলে → দ্রুত কাজ হয়  
**Cache Miss:** Cache-এ না পাওয়া গেলে RAM থেকে আনতে হয় → ধীর হয়

---

### 🔷 RAM — বিস্তারিত প্রকারভেদ

**RAM = Random Access Memory**
- **Volatile (উদ্বায়ী):** বিদ্যুৎ গেলে সব ডেটা মুছে যায়
- **Random Access:** যেকোনো ঠিকানায় সরাসরি অ্যাক্সেস করা যায়

| প্রকার | পূর্ণনাম | বৈশিষ্ট্য | ব্যবহার |
|---|---|---|---|
| **DRAM** | Dynamic RAM | Capacitor-এ চার্জ রেখে ডেটা সংরক্ষণ করে। বারবার Refresh করতে হয় (প্রতি মিলিসেকেন্ডে)। সস্তা কিন্তু ধীর। | Main Memory (Desktop/Laptop RAM) |
| **SRAM** | Static RAM | Flip-flop সার্কিটে ডেটা রাখে। Refresh লাগে না। দ্রুত কিন্তু দামি ও আকারে বড়। | Cache Memory (L1, L2, L3) |
| **SDRAM** | Synchronous DRAM | Clock signal-এর সাথে সিঙ্ক্রোনাইজড। DRAM-এর উন্নত সংস্করণ। | আধুনিক PC RAM |
| **DDR** | Double Data Rate | Clock-এর উভয় প্রান্তে (rising ও falling edge) ডেটা ট্রান্সফার করে → দ্বিগুণ গতি | আধুনিক PC/Laptop (DDR4, DDR5) |

---

### 🔷 ROM — বিস্তারিত প্রকারভেদ

**ROM = Read Only Memory**
- **Non-volatile (অউদ্বায়ী):** বিদ্যুৎ গেলেও ডেটা থাকে
- **ব্যবহার:** BIOS, Firmware, Microcontroller প্রোগ্রাম সংরক্ষণে

| প্রকার | পূর্ণনাম | বৈশিষ্ট্য | উদাহরণ |
|---|---|---|---|
| **ROM** | Read Only Memory | কারখানায় তৈরির সময় ডেটা লেখা হয়। কখনো পরিবর্তন করা যায় না। | পুরনো BIOS চিপ |
| **PROM** | Programmable ROM | একবার প্রোগ্রাম করা যায়, কিন্তু পরে মুছা যায় না। বিশেষ যন্ত্র (Programmer) দিয়ে লেখা হয়। | পুরনো ইলেকট্রনিক ডিভাইস |
| **EPROM** | Erasable Programmable ROM | UV (অতিবেগুনী) আলো দিয়ে মুছা যায়। মুছার পর পুনরায় প্রোগ্রাম করা যায়। কিন্তু UV আলোর মেশিন দরকার। | পুরনো Microcontroller |
| **EEPROM** | Electrically Erasable Programmable ROM | বৈদ্যুতিক সংকেত দিয়ে মুছা ও পুনরায় লেখা যায়। সার্কিটে থাকা অবস্থায়ই আপডেট করা যায়। | আধুনিক BIOS, স্মার্ট কার্ড |
| **Flash Memory** | — | EEPROM-এর উন্নত সংস্করণ। Block ধরে মুছা যায়, দ্রুত, ছোট আকার। | Pen Drive, SSD, Memory Card, Smartphone Storage |

---

## ১.৩ নম্বর পদ্ধতি — সম্পূর্ণ বিস্তারিত

### 🔷 চারটি নম্বর পদ্ধতি:

| পদ্ধতি | ভিত্তি (Base) | অঙ্কসমূহ | ব্যবহার |
|---|---|---|---|
| **Binary** | 2 | 0, 1 | কম্পিউটারের ভেতরে (সার্কিটে) |
| **Octal** | 8 | 0-7 | সংক্ষিপ্ত Binary representation |
| **Decimal** | 10 | 0-9 | মানুষের দৈনন্দিন ব্যবহার |
| **Hexadecimal** | 16 | 0-9, A-F | মেমোরি ঠিকানা, রঙের কোড (HTML) |

### 🔷 Hexadecimal মান টেবিল:
```
Decimal:  0  1  2  3  4  5  6  7  8  9  10  11  12  13  14  15
Hex:      0  1  2  3  4  5  6  7  8  9   A   B   C   D   E   F
Binary: 0000 0001 0010 0011 0100 0101 0110 0111 1000 1001 1010 1011 1100 1101 1110 1111
```

---

### 🔷 রূপান্তর পদ্ধতি — সম্পূর্ণ উদাহরণসহ

#### Binary → Decimal
প্রতিটি বিটকে 2-এর ঘাতে গুণ করো (ডানদিক থেকে শুরু, ঘাত = 0):

**উদাহরণ: 11001011 → ?**
```
অবস্থান:   7   6   5   4   3   2   1   0    (ডানদিক থেকে 0 শুরু)
বিট:       1   1   0   0   1   0   1   1
গুণফল:   128  64   0   0   8   0   2   1
যোগফল:  128 + 64 + 0 + 0 + 8 + 0 + 2 + 1 = 203
```
**উত্তর: (11001011)₂ = (203)₁₀**

#### Decimal → Binary (ভাগ পদ্ধতি)
সংখ্যাটিকে 2 দিয়ে ভাগ করতে থাকো, ভাগশেষগুলো নিচ থেকে উপরে পড়ো:

**উদাহরণ: 45 → Binary**
```
45 ÷ 2 = 22  ভাগশেষ  1   ↑ (উপরে পড়ো)
22 ÷ 2 = 11  ভাগশেষ  0   |
11 ÷ 2 = 5   ভাগশেষ  1   |
5  ÷ 2 = 2   ভাগশেষ  1   |
2  ÷ 2 = 1   ভাগশেষ  0   |
1  ÷ 2 = 0   ভাগশেষ  1   ↓ (নিচে শুরু)
উত্তর (নিচ থেকে উপরে): 101101
```
**উত্তর: (45)₁₀ = (101101)₂**

#### Decimal → Hexadecimal
সংখ্যাটিকে 16 দিয়ে ভাগ করতে থাকো:

**উদাহরণ: 255 → Hex**
```
255 ÷ 16 = 15  ভাগশেষ  15 = F
15  ÷ 16 = 0   ভাগশেষ  15 = F
উত্তর (নিচ থেকে উপরে): FF
```
**উত্তর: (255)₁₀ = (FF)₁₆**

#### Binary → Hexadecimal (সহজ পদ্ধতি)
বাম থেকে প্রতি 4টি বিট একটি Hex অঙ্কে রূপান্তর করো:

**উদাহরণ: 11110101 → Hex**
```
1111 | 0101
  F  |  5
উত্তর: F5
```

#### Octal → Binary
প্রতিটি Octal অঙ্ককে 3-বিট Binary-তে রূপান্তর:

**উদাহরণ: (75)₈**
```
7 = 111
5 = 101
উত্তর: (111101)₂
```

---

## ১.৪ লজিক গেট — সম্পূর্ণ বিস্তারিত

লজিক গেট হলো ডিজিটাল সার্কিটের মূল উপাদান। এগুলো Binary ইনপুট নিয়ে Binary আউটপুট দেয়।

### 🔷 সাতটি মৌলিক গেট:

#### AND গেট
- **নিয়ম:** সব ইনপুট 1 হলে আউটপুট 1, নইলে 0
- **বুলিয়ান:** Y = A · B (A AND B)

| A | B | A AND B |
|---|---|---|
| 0 | 0 | **0** |
| 0 | 1 | **0** |
| 1 | 0 | **0** |
| 1 | 1 | **1** |

#### OR গেট
- **নিয়ম:** যেকোনো একটি ইনপুট 1 হলে আউটপুট 1
- **বুলিয়ান:** Y = A + B (A OR B)

| A | B | A OR B |
|---|---|---|
| 0 | 0 | **0** |
| 0 | 1 | **1** |
| 1 | 0 | **1** |
| 1 | 1 | **1** |

#### NOT গেট (Inverter)
- **নিয়ম:** ইনপুটকে উল্টে দেয়
- **বুলিয়ান:** Y = Ā

| A | NOT A |
|---|---|
| 0 | **1** |
| 1 | **0** |

#### NAND গেট (Universal Gate)
- **নিয়ম:** AND-এর বিপরীত
- **বুলিয়ান:** Y = (A · B)'
- **কেন Universal?** শুধু NAND ব্যবহার করে AND, OR, NOT সব গেট তৈরি করা যায়

| A | B | NAND |
|---|---|---|
| 0 | 0 | **1** |
| 0 | 1 | **1** |
| 1 | 0 | **1** |
| 1 | 1 | **0** |

#### NOR গেট (Universal Gate)
- **নিয়ম:** OR-এর বিপরীত
- **বুলিয়ান:** Y = (A + B)'
- **কেন Universal?** শুধু NOR ব্যবহার করেও সব গেট তৈরি সম্ভব

| A | B | NOR |
|---|---|---|
| 0 | 0 | **1** |
| 0 | 1 | **0** |
| 1 | 0 | **0** |
| 1 | 1 | **0** |

#### XOR গেট (Exclusive OR)
- **নিয়ম:** ইনপুট দুটি আলাদা হলে 1, একই হলে 0
- **বুলিয়ান:** Y = A ⊕ B
- **ব্যবহার:** Half Adder, Parity Checker, Encryption

| A | B | XOR |
|---|---|---|
| 0 | 0 | **0** |
| 0 | 1 | **1** |
| 1 | 0 | **1** |
| 1 | 1 | **0** |

#### XNOR গেট (Exclusive NOR)
- **নিয়ম:** XOR-এর বিপরীত (ইনপুট একই হলে 1)
- **বুলিয়ান:** Y = (A ⊕ B)'

| A | B | XNOR |
|---|---|---|
| 0 | 0 | **1** |
| 0 | 1 | **0** |
| 1 | 0 | **0** |
| 1 | 1 | **1** |

> 📌 **গুরুত্বপূর্ণ:** NAND ও NOR কে **Universal Gate** বলা হয় কারণ এদের দিয়ে যেকোনো গেট তৈরি করা যায়। XOR গেটকে **"Odd Function"** বলা হয় কারণ বিজোড় সংখ্যক 1 থাকলে আউটপুট 1।

---

## ১.৫ কম্পিউটারের প্রজন্ম — বিস্তারিত

| প্রজন্ম | সময়কাল | প্রযুক্তি | বৈশিষ্ট্য | উদাহরণ |
|---|---|---|---|---|
| **১ম** | ১৯৪০-১৯৫৬ | Vacuum Tube | বিশাল আকার, প্রচুর তাপ, ঘন ঘন নষ্ট হতো, মেশিন ভাষায় প্রোগ্রাম | ENIAC, UNIVAC, IBM 701 |
| **২য়** | ১৯৫৬-১৯৬৩ | Transistor | ছোট আকার, কম তাপ, বেশি নির্ভরযোগ্য, Assembly ভাষা, COBOL/FORTRAN | IBM 1401, IBM 7090 |
| **৩য়** | ১৯৬৪-১৯৭১ | IC (Integrated Circuit) | আরো ছোট, High-level ভাষা (C, BASIC), Multiprocessing, OS শুরু | IBM 360, PDP-8 |
| **৪র্থ** | ১৯৭১-বর্তমান | VLSI Microprocessor | Personal Computer, GUI, Internet, Networking | Intel 4004, PC, Laptop |
| **৫ম** | বর্তমান-ভবিষ্যৎ | AI, Neural Network, Quantum | কৃত্রিম বুদ্ধিমত্তা, Machine Learning, Cloud Computing, Quantum Computing | Deep Learning Systems |

**📌 বাংলাদেশে প্রথম কম্পিউটার:** IBM-1620 (৩য় প্রজন্ম), বাংলাদেশ পরমাণু শক্তি কমিশন, **১৯৬৪ সালে** স্থাপিত।

---

## ১.৬ ইনপুট/আউটপুট ডিভাইস

### 🔷 ইনপুট ডিভাইস:
| ডিভাইস | কাজ |
|---|---|
| Keyboard | টেক্সট ও নির্দেশনা ইনপুট |
| Mouse | পয়েন্টার নিয়ন্ত্রণ |
| Scanner | ছবি ও ডকুমেন্ট ডিজিটাইজ করা |
| Webcam | ভিডিও ইনপুট |
| Microphone | অডিও ইনপুট |
| OMR | বহুনির্বাচনী উত্তরপত্র পড়া (Optical Mark Recognition) |
| OCR | ছাপানো টেক্সট পড়া (Optical Character Recognition) |
| Barcode Reader | পণ্যের বারকোড পড়া |
| Touch Screen | স্পর্শ-নির্ভর ইনপুট |

### 🔷 আউটপুট ডিভাইস:
| ডিভাইস | কাজ |
|---|---|
| Monitor | ভিজ্যুয়াল আউটপুট দেখানো |
| Printer | কাগজে প্রিন্ট করা |
| Speaker | শব্দ আউটপুট দেওয়া |
| Projector | বড় পর্দায় প্রজেকশন |
| Plotter | বড় আকারের ড্রয়িং প্রিন্ট |

---

---

# ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
# অধ্যায় ২: কম্পিউটার নেটওয়ার্কিং
### 🔴 সর্বোচ্চ গুরুত্ব (~২২%)
# ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

---

## ২.১ OSI Model — সম্পূর্ণ বিস্তারিত

**OSI = Open Systems Interconnection**
**তৈরি:** ISO (International Organization for Standardization) কর্তৃক ১৯৮৪ সালে।
**উদ্দেশ্য:** ভিন্ন ভিন্ন কোম্পানির ডিভাইস ও সফটওয়্যার একে অপরের সাথে যোগাযোগ করতে পারে তা নিশ্চিত করা।

### 🔷 মুখস্থের সহজ উপায়:
**"All People Seem To Need Data Processing"**  
(Application, Presentation, Session, Transport, Network, Data Link, Physical)

অথবা উল্টো (Physical থেকে): **"Please Do Not Throw Sausage Pizza Away"**

---

### 🔷 OSI-এর ৭টি স্তর — বিস্তারিত:

#### স্তর ৭ — Application Layer (অ্যাপ্লিকেশন স্তর)
- **কাজ:** ব্যবহারকারী ও নেটওয়ার্কের মধ্যে ইন্টারফেস প্রদান। সরাসরি ব্যবহারকারীর সাথে কথা বলে।
- **সেবা:** Email, Web Browsing, File Transfer, DNS lookup
- **প্রোটোকল:** HTTP, HTTPS, FTP, SMTP, POP3, IMAP, DNS, DHCP, Telnet, SSH
- **উদাহরণ:** ব্রাউজারে www.google.com টাইপ করলে এই স্তর কাজ শুরু করে

#### স্তর ৬ — Presentation Layer (প্রেজেন্টেশন স্তর)
- **কাজ:** ডেটার ফরম্যাট নির্ধারণ, এনক্রিপশন/ডিক্রিপশন, কম্প্রেশন
- **কাজের তালিকা:**
  - **Translation:** ভিন্ন ফরম্যাটের ডেটা রূপান্তর (যেমন EBCDIC → ASCII)
  - **Encryption:** নিরাপদ ট্রান্সমিশনের জন্য ডেটা এনক্রিপ্ট করা
  - **Compression:** ডেটার আকার ছোট করা
- **প্রোটোকল/ফরম্যাট:** SSL, TLS, JPEG, PNG, MP4, MP3, ASCII, Unicode

#### স্তর ৫ — Session Layer (সেশন স্তর)
- **কাজ:** দুটি ডিভাইসের মধ্যে যোগাযোগের সেশন তৈরি, পরিচালনা ও সমাপ্তি
- **কাজের তালিকা:**
  - **Session Establishment:** সেশন শুরু করা
  - **Session Maintenance:** সেশন চলমান রাখা
  - **Session Termination:** সেশন শেষ করা
  - **Synchronization:** Checkpoints রাখা যাতে ব্যর্থতায় পুনরায় শুরু করা যায়
- **প্রোটোকল:** NetBIOS, RPC (Remote Procedure Call), NFS

#### স্তর ৪ — Transport Layer (ট্রান্সপোর্ট স্তর)
- **কাজ:** নির্ভরযোগ্য ডেটা ট্রান্সফার, Flow Control, Error Control
- **ইউনিট:** **Segment** (TCP) বা **Datagram** (UDP)
- **গুরুত্বপূর্ণ কাজ:**
  - **Segmentation:** বড় ডেটাকে ছোট ছোট Segment-এ ভাগ করা
  - **Multiplexing:** একই সংযোগে একাধিক অ্যাপ্লিকেশনের ডেটা পাঠানো (Port নম্বর দিয়ে)
  - **Flow Control:** রিসিভার অভিভূত না হয় তা নিশ্চিত করা
  - **Error Detection:** ডেটা ঠিকঠাক পৌঁছেছে কিনা যাচাই
- **প্রোটোকল:** TCP, UDP

#### স্তর ৩ — Network Layer (নেটওয়ার্ক স্তর)
- **কাজ:** ভিন্ন নেটওয়ার্কের মধ্যে ডেটা রাউটিং, লজিক্যাল অ্যাড্রেসিং (IP)
- **ইউনিট:** **Packet**
- **গুরুত্বপূর্ণ কাজ:**
  - **Routing:** উৎস থেকে গন্তব্যে সর্বোত্তম পথ নির্ধারণ
  - **IP Addressing:** প্রতিটি ডিভাইসকে লজিক্যাল ঠিকানা দেওয়া
  - **Fragmentation:** Packet ছোট করা প্রয়োজনে
- **প্রোটোকল:** IP (IPv4, IPv6), ICMP, IGMP, ARP
- **ডিভাইস:** Router

#### স্তর ২ — Data Link Layer (ডেটা লিংক স্তর)
- **কাজ:** ফিজিক্যাল স্তরের ভুল সংশোধন, MAC অ্যাড্রেসিং, ফ্রেম তৈরি
- **ইউনিট:** **Frame**
- **দুটি উপস্তর:**
  - **LLC (Logical Link Control):** উচ্চতর স্তরের সাথে ইন্টারফেস
  - **MAC (Media Access Control):** ফিজিক্যাল মিডিয়া অ্যাক্সেস নিয়ন্ত্রণ
- **প্রোটোকল:** Ethernet, PPP, HDLC, Wi-Fi (802.11), ARP
- **ডিভাইস:** Switch, Bridge, NIC (Network Interface Card)

#### স্তর ১ — Physical Layer (ফিজিক্যাল স্তর)
- **কাজ:** বিট (0 ও 1) হিসেবে কাঁচা ডেটা ফিজিক্যাল মাধ্যমে প্রেরণ
- **ইউনিট:** **Bit**
- **কাজের তালিকা:**
  - বিট এনকোডিং (ভোল্টেজ, আলো, রেডিও তরঙ্গে রূপান্তর)
  - ট্রান্সমিশন মোড (Simplex, Half-duplex, Full-duplex)
  - ক্যাবল টাইপ নির্ধারণ
- **মাধ্যম:** Twisted Pair, Coaxial, Fiber Optic, Wireless
- **ডিভাইস:** Hub, Repeater, Modem

---

## ২.২ TCP/IP Model — বিস্তারিত

TCP/IP হলো ইন্টারনেটের বাস্তব প্রোটোকল সমষ্টি। OSI একটি তাত্ত্বিক মডেল, কিন্তু TCP/IP বাস্তবে ইন্টারনেট চালায়।

| TCP/IP স্তর | OSI সমতুল্য | প্রোটোকল/ডিভাইস | কাজ |
|---|---|---|---|
| **Application** | 7 + 6 + 5 (Application + Presentation + Session) | HTTP, FTP, DNS, SMTP, SSH | ব্যবহারকারীর সাথে সরাসরি কথা বলে |
| **Transport** | 4 (Transport) | TCP, UDP | নির্ভরযোগ্য ডেলিভারি নিশ্চিত করে |
| **Internet** | 3 (Network) | IP, ICMP, ARP | রাউটিং ও IP অ্যাড্রেসিং |
| **Network Access** | 2 + 1 (Data Link + Physical) | Ethernet, Wi-Fi, ARP | ফিজিক্যাল ট্রান্সমিশন |

---

### 🔷 TCP vs UDP — সম্পূর্ণ তুলনা

| বৈশিষ্ট্য | TCP (Transmission Control Protocol) | UDP (User Datagram Protocol) |
|---|---|---|
| **সংযোগ পদ্ধতি** | Connection-oriented (3-way Handshake) | Connectionless (কোনো হ্যান্ডশেক নেই) |
| **নির্ভরযোগ্যতা** | সম্পূর্ণ নির্ভরযোগ্য (ACK নিশ্চিত করে) | অনির্ভরযোগ্য (কোনো নিশ্চয়তা নেই) |
| **ডেটার ক্রম** | ক্রম নিশ্চিত করে (Sequence Number) | ক্রমের নিশ্চয়তা নেই |
| **গতি** | ধীর (overhead বেশি) | দ্রুত (overhead কম) |
| **Header আকার** | ২০ bytes (ন্যূনতম) | ৮ bytes (ছোট) |
| **Flow Control** | আছে | নেই |
| **Error Checking** | আছে ও সংশোধন করে | শুধু Detection (সংশোধন নয়) |
| **ব্যবহার** | Web (HTTP), Email, File Transfer, Banking | DNS, Video Streaming, VoIP, Online Gaming |

#### TCP 3-Way Handshake (সংযোগ স্থাপন):
```
Client                          Server
  │                               │
  │──── SYN (সংযোগ চাই) ────────▶│
  │                               │
  │◀─── SYN-ACK (ঠিক আছে, তুমি?) ┤
  │                               │
  │──── ACK (ধন্যবাদ, সংযুক্ত) ──▶│
  │                               │
  │══════ ডেটা ট্রান্সফার ════════│
```

---

## ২.৩ নেটওয়ার্ক ডিভাইস — বিস্তারিত

| ডিভাইস | OSI স্তর | কাজ | বিশেষত্ব |
|---|---|---|---|
| **Hub** | Physical (১) | সব পোর্টে ডেটা Broadcast করে | বুদ্ধিহীন, Collision হয়, পুরনো প্রযুক্তি |
| **Repeater** | Physical (১) | দুর্বল সিগন্যাল পুনরুজ্জীবিত করে দূরত্ব বাড়ায় | শুধু সিগন্যাল শক্তি বাড়ায়, ডেটা বিশ্লেষণ করে না |
| **Bridge** | Data Link (২) | দুটি LAN সেগমেন্ট যুক্ত করে, MAC দেখে ফরোয়ার্ড করে | Collision Domain ভাগ করে |
| **Switch** | Data Link (২) | MAC অ্যাড্রেস টেবিল দেখে নির্দিষ্ট পোর্টে পাঠায় | Hub-এর চেয়ে বুদ্ধিমান, Collision কম |
| **Router** | Network (৩) | IP দেখে ভিন্ন নেটওয়ার্কে Routing করে | LAN-কে Internet-এ যুক্ত করে |
| **Gateway** | সব স্তর | সম্পূর্ণ ভিন্ন প্রোটোকলের নেটওয়ার্ক সংযুক্ত করে | Protocol Translator হিসেবে কাজ করে |
| **Modem** | Physical (১) | ডিজিটাল → অ্যানালগ এবং অ্যানালগ → ডিজিটাল রূপান্তর | Modulator + Demodulator |
| **NIC** | Data Link (২) | কম্পিউটারকে নেটওয়ার্কে সংযুক্ত করে | MAC অ্যাড্রেস ধারণ করে |
| **Firewall** | Network/Transport | নেটওয়ার্ক ট্রাফিক ফিল্টার করে নিরাপত্তা দেয় | Packet Filtering, Stateful Inspection |

### 🔷 গুরুত্বপূর্ণ পার্থক্য:
- **Hub vs Switch:** Hub সবার কাছে পাঠায়, Switch শুধু নির্দিষ্ট প্রাপকের কাছে
- **Switch vs Router:** Switch একই নেটওয়ার্কে (MAC দিয়ে), Router ভিন্ন নেটওয়ার্কে (IP দিয়ে)
- **Node:** নেটওয়ার্কে সংযুক্ত যেকোনো ডিভাইস (PC, Phone, Printer, Server)
- **Backbone:** বিভিন্ন নেটওয়ার্ককে যুক্ত করার প্রধান হাইস্পিড পথ

---

## ২.৪ নেটওয়ার্ক টোপোলজি — বিস্তারিত

| টোপোলজি | কাঠামো | সুবিধা | অসুবিধা | ব্যবহার |
|---|---|---|---|---|
| **Bus** | একটি মূল ক্যাবলে সব ডিভাইস সংযুক্ত | সহজ, সস্তা, কম ক্যাবল | একটি সংযোগ নষ্ট হলে সব বিচ্ছিন্ন, Collision বেশি | ছোট নেটওয়ার্ক |
| **Star** | কেন্দ্রীয় Hub/Switch এ সব সংযুক্ত | একটি নষ্ট হলে বাকি চলে, সমস্যা চিহ্নিত সহজ | Hub/Switch নষ্ট হলে সব বন্ধ, বেশি ক্যাবল | আধুনিক অফিস নেটওয়ার্ক |
| **Ring** | বৃত্তাকারে প্রতিটি ডিভাইস পরের সাথে যুক্ত | সমান গতি বণ্টন, Collision নেই | একটি নষ্ট হলে পুরো নেটওয়ার্ক বন্ধ | পুরনো Token Ring |
| **Mesh** | প্রতিটি ডিভাইসের সাথে প্রতিটির সরাসরি সংযোগ | অত্যন্ত নির্ভরযোগ্য, কোনো Single Point of Failure নেই | অত্যন্ত ব্যয়বহুল, জটিল | Military, Critical Systems |
| **Tree** | Bus ও Star-এর মিশ্রণ (Star গুলো Bus-এ যুক্ত) | Scalable, Hierarchical | Root নষ্ট হলে সমস্যা | বড় প্রতিষ্ঠান |
| **Hybrid** | দুই বা ততোধিক টোপোলজির মিশ্রণ | নমনীয় | জটিল | বড় কর্পোরেট নেটওয়ার্ক |

**Mesh-এ সংযোগ সংখ্যা:** n ডিভাইস হলে = n(n-1)/2 সংযোগ

---

## ২.৫ নেটওয়ার্কের প্রকারভেদ (ভৌগোলিক এলাকা অনুযায়ী)

| প্রকার | পূর্ণনাম | পরিসীমা | বৈশিষ্ট্য | উদাহরণ |
|---|---|---|---|---|
| **PAN** | Personal Area Network | ~১০ মিটার | ব্যক্তিগত ডিভাইস সংযোগ | Bluetooth, USB |
| **LAN** | Local Area Network | একটি বিল্ডিং/ক্যাম্পাস | দ্রুততম, ব্যক্তিগত মালিকানা | অফিস, স্কুল নেটওয়ার্ক |
| **MAN** | Metropolitan Area Network | একটি শহর | LAN-এর চেয়ে বড় | শহরের ক্যাবল TV, ISP |
| **WAN** | Wide Area Network | দেশ বা বৈশ্বিক | ধীর, সরকার/কোম্পানি পরিচালিত | Internet |

---

## ২.৬ গুরুত্বপূর্ণ প্রোটোকল ও পোর্ট নম্বর — সম্পূর্ণ তালিকা

| প্রোটোকল | পূর্ণরূপ | পোর্ট | ট্রান্সপোর্ট | কাজ |
|---|---|---|---|---|
| **HTTP** | HyperText Transfer Protocol | **80** | TCP | ওয়েবপেজ ট্রান্সফার (নিরাপত্তাহীন) |
| **HTTPS** | HTTP Secure | **443** | TCP | SSL/TLS সহ নিরাপদ ওয়েব |
| **FTP** | File Transfer Protocol | **21** (Control), 20 (Data) | TCP | ফাইল আপলোড/ডাউনলোড |
| **SSH** | Secure Shell | **22** | TCP | নিরাপদ রিমোট কমান্ড অ্যাক্সেস |
| **Telnet** | — | **23** | TCP | রিমোট অ্যাক্সেস (অনিরাপদ, SSH দিয়ে প্রতিস্থাপিত) |
| **SMTP** | Simple Mail Transfer Protocol | **25** | TCP | ইমেইল পাঠানো (Sending) |
| **DNS** | Domain Name System | **53** | UDP/TCP | Domain নাম → IP রূপান্তর |
| **DHCP** | Dynamic Host Configuration Protocol | **67** (Server), 68 (Client) | UDP | স্বয়ংক্রিয়ভাবে IP দেওয়া |
| **POP3** | Post Office Protocol 3 | **110** | TCP | ইমেইল রিসিভ (সার্ভার থেকে মুছে ফেলে) |
| **IMAP** | Internet Message Access Protocol | **143** | TCP | ইমেইল রিসিভ (সার্ভারে রেখে দেয়) |
| **SNMP** | Simple Network Management Protocol | **161** | UDP | নেটওয়ার্ক ডিভাইস পর্যবেক্ষণ |
| **RDP** | Remote Desktop Protocol | **3389** | TCP | Windows রিমোট ডেস্কটপ |

> 📌 **মুখস্থের টিপস:** 20/21=FTP, 22=SSH, 23=Telnet, 25=SMTP, 53=DNS, 67/68=DHCP, 80=HTTP, 110=POP3, 143=IMAP, 443=HTTPS

---

## ২.৭ IP Address — বিস্তারিত

### 🔷 IPv4 vs IPv6:

| বৈশিষ্ট্য | IPv4 | IPv6 |
|---|---|---|
| **বিট সংখ্যা** | 32-bit | 128-bit |
| **লেখার পদ্ধতি** | Dotted Decimal (192.168.1.1) | Hexadecimal (2001:0db8::1) |
| **মোট ঠিকানা** | ~4.3 বিলিয়ন | ~340 অন্ডেসিলিয়ন (অক্ষরণীয় বিশাল) |
| **NAT দরকার** | হ্যাঁ (IP সংকটের কারণে) | না |
| **Header আকার** | 20-60 bytes | 40 bytes (fixed) |

### 🔷 IPv4 Class:

| Class | প্রথম অক্টেটের রেঞ্জ | Network/Host বিট | ব্যবহার |
|---|---|---|---|
| **A** | 1-126 | 8 Network / 24 Host | বড় নেটওয়ার্ক (ISP, Government) |
| **B** | 128-191 | 16 Network / 16 Host | মাঝারি নেটওয়ার্ক (বিশ্ববিদ্যালয়) |
| **C** | 192-223 | 24 Network / 8 Host | ছোট নেটওয়ার্ক (অফিস) |
| **D** | 224-239 | — | Multicast |
| **E** | 240-255 | — | গবেষণায় সংরক্ষিত |

**Private IP Range (Internet-এ রাউট হয় না):**
- Class A: 10.0.0.0 – 10.255.255.255
- Class B: 172.16.0.0 – 172.31.255.255
- Class C: 192.168.0.0 – 192.168.255.255
- Loopback: 127.0.0.1 (localhost)

---

## ২.৮ ওয়্যারলেস প্রযুক্তি — বিস্তারিত

| প্রযুক্তি | IEEE মান | পরিসীমা | ডেটা রেট | বৈশিষ্ট্য |
|---|---|---|---|---|
| **WiFi** | 802.11 (a/b/g/n/ac/ax) | 30-100 মিটার | 11 Mbps – 10+ Gbps | ওয়্যারলেস LAN, রাউটার |
| **Bluetooth** | 802.15 | ~10 মিটার | 1-24 Mbps | পিকোনেটে সর্বোচ্চ **৭টি Slave** + 1 Master |
| **WiMAX** | 802.16 | ~50 কিমি | 70 Mbps পর্যন্ত | Wireless MAN, Broadband |
| **Infrared** | IrDA | ~1 মিটার | 1-4 Mbps | TV Remote, পুরনো ডিভাইস |
| **4G/LTE** | — | কয়েক কিমি | 100 Mbps পর্যন্ত | মোবাইল ইন্টারনেট |
| **5G** | — | কয়েকশ মিটার | 1-20 Gbps | আধুনিক মোবাইল, IoT |
| **NFC** | — | ~4 সেমি | 424 Kbps | Contactless payment, Card tap |

> 📌 **পরীক্ষার গুরুত্বপূর্ণ তথ্য:**
> - Bluetooth পিকোনেটে সর্বোচ্চ **৭টি Slave** ডিভাইস থাকে
> - WiFi এর IEEE মান = **802.11**
> - WiMAX = **Worldwide Interoperability for Microwave Access**
> - LAN-এ সর্বোচ্চ **৪টি** Repeater ব্যবহার করা যায়

---

## ২.৯ Transmission Media (ট্রান্সমিশন মাধ্যম)

### 🔷 Guided Media (তারযুক্ত):

| মাধ্যম | বৈশিষ্ট্য | গতি | দূরত্ব |
|---|---|---|---|
| **Twisted Pair (UTP/STP)** | সস্তা, সহজলভ্য, Electromagnetic interference হয় | 10 Mbps – 10 Gbps | 100 মিটার পর্যন্ত |
| **Coaxial Cable** | টিভি তার, বেশি শিল্ডিং | 10-500 Mbps | কয়েকশ মিটার |
| **Fiber Optic** | আলোক সংকেত ব্যবহার করে, EMI নেই, সবচেয়ে দ্রুত | 100 Gbps+ | কয়েকশ কিমি |

### 🔷 Unguided Media (ওয়্যারলেস):
- Radio Wave, Microwave, Infrared, Satellite

---

---

# ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
# অধ্যায় ৩: ডেটাবেজ ম্যানেজমেন্ট সিস্টেম (DBMS)
### 🔴 সর্বোচ্চ গুরুত্ব (~২০%)
# ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

---

## ৩.১ DBMS মৌলিক ধারণা — বিস্তারিত

### 🔷 DBMS কী?
**DBMS (Database Management System)** হলো একটি সফটওয়্যার সিস্টেম যা ডেটা সংগঠিতভাবে সংরক্ষণ, পুনরুদ্ধার, আপডেট ও মুছতে সাহায্য করে।

**ফাইল সিস্টেম vs DBMS:**
- পুরনো পদ্ধতিতে ডেটা সরাসরি ফাইলে রাখা হতো — এতে ডেটার পুনরাবৃত্তি, অসামঞ্জস্য ও নিরাপত্তার সমস্যা ছিল।
- DBMS এই সমস্যাগুলো সমাধান করে।

### 🔷 DBMS-এর সুবিধা:
- **Data Redundancy হ্রাস:** একই ডেটা বারবার সংরক্ষণ করতে হয় না
- **Data Consistency:** একটি জায়গায় পরিবর্তন করলে সব জায়গায় আপডেট হয়
- **Data Integrity:** ভুল ডেটা প্রবেশ রোধ করে (Constraints দিয়ে)
- **Data Security:** ব্যবহারকারীভিত্তিক অ্যাক্সেস নিয়ন্ত্রণ
- **Concurrent Access:** একাধিক ব্যবহারকারী একই সময়ে ডেটা ব্যবহার করতে পারে

### 🔷 DBMS vs RDBMS — বিস্তারিত:
| বৈশিষ্ট্য | DBMS | RDBMS |
|---|---|---|
| **ডেটা সংরক্ষণ** | ফাইল আকারে (হায়ারার্কিক্যাল বা নেটওয়ার্ক) | টেবিল (Relation) আকারে |
| **সম্পর্ক** | টেবিলের মধ্যে কোনো সম্পর্ক নেই | Foreign Key দিয়ে টেবিলে সম্পর্ক |
| **ACID** | সমর্থন করে না বা আংশিক | সম্পূর্ণ ACID সমর্থন |
| **SQL** | ব্যবহার করে না | SQL ব্যবহার করে |
| **নরমালাইজেশন** | নেই | আছে |
| **Data Integrity** | কম | বেশি |
| **উদাহরণ** | XML Database, IMS | MySQL, Oracle, PostgreSQL, SQL Server |

---

## ৩.২ DDBMS — বিস্তারিত

**📌 বাংলাদেশ ব্যাংক AME 2019 পরীক্ষায় এসেছিল!**

### 🔷 DDBMS (Distributed Database Management System) কী?
একটি DDBMS হলো এমন একটি সিস্টেম যেখানে ডেটাবেজ একটি কম্পিউটারে নয়, বরং **নেটওয়ার্কে সংযুক্ত একাধিক কম্পিউটারে** বিতরণ করা থাকে। ব্যবহারকারীর কাছে এটি একটি একক ডেটাবেজের মতো মনে হয়।

**উদাহরণ:** বাংলাদেশ ব্যাংকের ATM নেটওয়ার্ক — ঢাকা, চট্টগ্রাম, সিলেটে আলাদা ডেটাবেজ সার্ভার কিন্তু সব একসাথে কাজ করে।

### 🔷 DDBMS-এর বৈশিষ্ট্য:
| বৈশিষ্ট্য | ব্যাখ্যা |
|---|---|
| **Location Transparency** | ডেটা কোথায় আছে জানার দরকার নেই |
| **Replication Transparency** | ডেটা একাধিক স্থানে কপি হলেও ব্যবহারকারী বোঝে না |
| **Fragmentation Transparency** | ডেটা বিভিন্ন ভাগে থাকলেও একটি টেবিলের মতো দেখায় |
| **Hardware Independence** | বিভিন্ন ধরনের হার্ডওয়ারে চলতে পারে |
| **OS Independence** | বিভিন্ন অপারেটিং সিস্টেমে কাজ করে |
| **Network Independence** | বিভিন্ন নেটওয়ার্ক প্রোটোকলে চলে |
| **DBMS Independence** | বিভিন্ন DBMS সফটওয়্যারে কাজ করে |
| **Distributed Transaction** | একাধিক সাইটে লেনদেন একসাথে পরিচালনা |

### 🔷 DDBMS-এর সুবিধা:
- ডেটা স্থানীয়ভাবে পাওয়া যায় → দ্রুত
- একটি সাইট নষ্ট হলে অন্য সাইট চলে → নির্ভরযোগ্য
- নতুন সাইট সহজে যোগ করা যায় → Scalable

### 🔷 DDBMS-এর অসুবিধা:
- ডিজাইন জটিল
- নিরাপত্তা নিশ্চিত করা কঠিন
- নেটওয়ার্ক সমস্যায় ডেটা সামঞ্জস্য রক্ষা কঠিন

---

## ৩.৩ SQL — সম্পূর্ণ বিস্তারিত

### 🔷 SQL-এর চারটি প্রধান ভাগ:

#### DDL — Data Definition Language
ডেটাবেজের কাঠামো তৈরি ও পরিবর্তনে ব্যবহৃত। এই কমান্ডগুলো Auto-commit হয়।

```sql
-- টেবিল তৈরি
CREATE TABLE employees (
    emp_id   INT          PRIMARY KEY,
    name     VARCHAR(100) NOT NULL,
    salary   DECIMAL(10,2),
    dept_id  INT,
    FOREIGN KEY (dept_id) REFERENCES department(dept_id)
);

-- টেবিলে নতুন কলাম যোগ
ALTER TABLE employees ADD COLUMN email VARCHAR(100);

-- কলাম পরিবর্তন
ALTER TABLE employees MODIFY COLUMN name VARCHAR(150);

-- কলাম মুছে ফেলা
ALTER TABLE employees DROP COLUMN email;

-- পুরো টেবিল মুছে ফেলা (structure ও data দুটোই)
DROP TABLE employees;

-- শুধু ডেটা মুছা (structure থাকে)
TRUNCATE TABLE employees;
```

#### DML — Data Manipulation Language
ডেটা যোগ, পরিবর্তন, মুছা ও পড়ার জন্য। Rollback করা যায়।

```sql
-- ডেটা ঢোকানো
INSERT INTO employees (emp_id, name, salary, dept_id)
VALUES (1, 'Rahim', 50000.00, 3);

-- একাধিক সারি একসাথে
INSERT INTO employees VALUES
    (2, 'Karim', 60000.00, 2),
    (3, 'Salma', 55000.00, 1);

-- ডেটা খোঁজা
SELECT name, salary
FROM employees
WHERE salary > 50000
ORDER BY salary DESC;

-- সব কলাম দেখা
SELECT * FROM employees;

-- শর্তসহ
SELECT * FROM employees
WHERE dept_id = 3 AND salary BETWEEN 40000 AND 70000;

-- ডেটা আপডেট
UPDATE employees
SET salary = salary * 1.10   -- ১০% বেতন বৃদ্ধি
WHERE dept_id = 2;

-- ডেটা মুছা
DELETE FROM employees WHERE emp_id = 5;
```

#### DCL — Data Control Language
নিরাপত্তা ও অ্যাক্সেস নিয়ন্ত্রণ:

```sql
-- ব্যবহারকারীকে অনুমতি দেওয়া
GRANT SELECT, INSERT ON employees TO 'user1'@'localhost';

-- অনুমতি প্রত্যাহার
REVOKE INSERT ON employees FROM 'user1'@'localhost';
```

#### TCL — Transaction Control Language
লেনদেন পরিচালনা:

```sql
-- লেনদেন শুরু
BEGIN TRANSACTION;

UPDATE accounts SET balance = balance - 5000 WHERE acc_no = '001';
UPDATE accounts SET balance = balance + 5000 WHERE acc_no = '002';

-- সফল হলে সংরক্ষণ
COMMIT;

-- ব্যর্থ হলে বাতিল
ROLLBACK;
```

---

### 🔷 JOIN — বিস্তারিত উদাহরণসহ

```sql
-- মনে করি দুটি টেবিল:
-- Student: (id, name, dept_id)
-- Department: (dept_id, dept_name)

-- INNER JOIN: উভয় টেবিলে মিলে এমন রেকর্ড
SELECT s.name, d.dept_name
FROM student s
INNER JOIN department d ON s.dept_id = d.dept_id;
-- শুধু যে students-এর dept_id, department টেবিলে আছে তারা

-- LEFT JOIN: বাম টেবিলের সব + ডানে না থাকলে NULL
SELECT s.name, d.dept_name
FROM student s
LEFT JOIN department d ON s.dept_id = d.dept_id;
-- সব students দেখাবে, dept না থাকলে NULL

-- RIGHT JOIN: ডান টেবিলের সব
SELECT s.name, d.dept_name
FROM student s
RIGHT JOIN department d ON s.dept_id = d.dept_id;

-- FULL OUTER JOIN: উভয় টেবিলের সব
SELECT s.name, d.dept_name
FROM student s
FULL OUTER JOIN department d ON s.dept_id = d.dept_id;
```

### 🔷 Aggregate Function:
```sql
SELECT COUNT(*) FROM employees;           -- মোট সারি গণনা
SELECT SUM(salary) FROM employees;        -- বেতনের যোগফল
SELECT AVG(salary) FROM employees;        -- গড় বেতন
SELECT MAX(salary) FROM employees;        -- সর্বোচ্চ বেতন
SELECT MIN(salary) FROM employees;        -- সর্বনিম্ন বেতন

-- GROUP BY দিয়ে
SELECT dept_id, COUNT(*), AVG(salary)
FROM employees
GROUP BY dept_id
HAVING AVG(salary) > 50000;   -- HAVING মানে GROUP BY-এর পরে WHERE
```

---

## ৩.৪ Normalization — সম্পূর্ণ বিস্তারিত

**লক্ষ্য:** ডেটা পুনরাবৃত্তি (Redundancy) ও Update Anomaly দূর করা।

### 🔷 Anomaly (অসামঞ্জস্য) কী?
- **Insert Anomaly:** নতুন ডেটা রাখতে সমস্যা
- **Update Anomaly:** একটি জায়গায় পরিবর্তন করলে অন্য জায়গায় ভুল থাকে
- **Delete Anomaly:** একটি রেকর্ড মুছলে অন্য দরকারি তথ্যও মুছে যায়

---

#### 1NF (First Normal Form) — প্রথম স্বাভাবিক রূপ
**শর্ত:**
1. প্রতিটি কলামে একটিমাত্র মান (Atomic Value) — কোনো List বা Set থাকবে না
2. একই রকম কলাম গ্রুপ থাকবে না (Repeating Group নেই)
3. প্রতিটি সারি অনন্য (Primary Key আছে)

**লঙ্ঘনের উদাহরণ:**
```
Student(id, name, courses)
1, "Rahim", "Math, Physics, Chemistry"  ← একটি কলামে তিনটি মান — 1NF লঙ্ঘন
```
**সমাধান:** আলাদা সারি করো।

#### 2NF (Second Normal Form) — দ্বিতীয় স্বাভাবিক রূপ
**শর্ত:** 1NF পূরণ + **Partial Dependency দূর করতে হবে**
- Partial Dependency = কোনো non-key attribute যদি Composite Primary Key-এর মাত্র একটি অংশের উপর নির্ভরশীল হয়

**লঙ্ঘনের উদাহরণ:**
```
Order(order_id, product_id, product_name, quantity)
Primary Key = (order_id, product_id)
product_name শুধু product_id-এর উপর নির্ভরশীল → 2NF লঙ্ঘন
```
**সমাধান:** পৃথক Product টেবিল তৈরি করো।

#### 3NF (Third Normal Form) — তৃতীয় স্বাভাবিক রূপ
**শর্ত:** 2NF পূরণ + **Transitive Dependency দূর করতে হবে**
- Transitive Dependency = Non-key attribute যদি অন্য non-key attribute-এর উপর নির্ভরশীল হয়

**লঙ্ঘনের উদাহরণ:**
```
Student(id, name, zip_code, city)
city নির্ভরশীল zip_code-এর উপর → zip_code নির্ভরশীল id-এর উপর → Transitive Dependency
```
**সমাধান:** আলাদা ZipCode টেবিল।

#### BCNF (Boyce-Codd Normal Form)
**শর্ত:** 3NF-এর কঠোর সংস্করণ।  
প্রতিটি Determinant-কে Candidate Key হতে হবে।

> **মনে রাখো:** 1NF → 2NF → 3NF → BCNF → 4NF → 5NF (পরীক্ষায় সাধারণত 1NF-3NF পর্যন্তই আসে)

---

## ৩.৫ ACID Properties — সম্পূর্ণ বিস্তারিত

**ACID** হলো Database Transaction-এর চারটি মূল বৈশিষ্ট্য যা ডেটার নির্ভরযোগ্যতা নিশ্চিত করে।

| বৈশিষ্ট্য | ইংরেজি নাম | বিস্তারিত ব্যাখ্যা | উদাহরণ |
|---|---|---|---|
| **A** | **Atomicity** | পুরো লেনদেন হয় সম্পূর্ণ হবে, না হয় কিছুই হবে না। মাঝপথে থামলে সব ফিরিয়ে নেওয়া হবে (Rollback)। | ব্যাংক ট্রান্সফার: টাকা কাটা হলো কিন্তু জমা হলো না → Rollback করে পুরোটাই বাতিল |
| **C** | **Consistency** | লেনদেনের আগে ও পরে ডেটাবেজ সবসময় বৈধ অবস্থায় থাকবে। সব নিয়ম (Constraints) মানা হবে। | Balance কখনো নেগেটিভ হবে না (যদি Constraint থাকে) |
| **I** | **Isolation** | একটি চলমান লেনদেন অন্য লেনদেনের উপর প্রভাব ফেলবে না। প্রতিটি লেনদেন স্বাধীনভাবে চলবে। | দুজন একই সময়ে একই আসন বুক করলে একজনই পাবে |
| **D** | **Durability** | Commit হওয়া লেনদেন স্থায়ীভাবে সংরক্ষিত থাকবে। বিদ্যুৎ গেলেও তথ্য থাকবে (Log-এ লেখা হয়)। | Commit-এর পর সার্ভার ক্র্যাশ করলেও ডেটা নিরাপদ |

---

## ৩.৬ Key — সম্পূর্ণ প্রকারভেদ

| Key | সংজ্ঞা | বৈশিষ্ট্য |
|---|---|---|
| **Primary Key** | টেবিলের প্রতিটি সারিকে অনন্যভাবে শনাক্ত করে | NULL হতে পারে না, পরিবর্তন করা উচিত নয় |
| **Foreign Key** | অন্য টেবিলের Primary Key-এর রেফারেন্স | Referential Integrity বজায় রাখে |
| **Candidate Key** | Primary Key হওয়ার যোগ্য (Unique + NOT NULL) | একাধিক থাকতে পারে, একটি Primary হয় |
| **Alternate Key** | Candidate Key যেটা Primary হয়নি | — |
| **Super Key** | যেকোনো কলামের সমষ্টি যা অনন্যভাবে শনাক্ত করে | Candidate Key + অতিরিক্ত কলাম |
| **Composite Key** | দুই বা ততোধিক কলাম মিলে Primary Key | প্রতিটি কলাম আলাদাভাবে অনন্য নয় |
| **Unique Key** | অনন্য মান রাখে কিন্তু NULL থাকতে পারে | একটি টেবিলে একাধিক থাকতে পারে |

---

---

# ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
# অধ্যায় ৪: প্রোগ্রামিং ও সফটওয়্যার ইঞ্জিনিয়ারিং
### 🔴 সর্বোচ্চ গুরুত্ব (~১৮%)
# ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

---

## ৪.১ OOP — সম্পূর্ণ বিস্তারিত

**OOP = Object-Oriented Programming**
কম্পিউটার প্রোগ্রামকে বাস্তব জগতের বস্তু ও তাদের আচরণের ভিত্তিতে সংগঠিত করার পদ্ধতি।

### 🔷 মূল ধারণা:
- **Class:** বস্তুর নকশা বা ছাঁচ (Blueprint)। যেমন: "Car" একটি Class।
- **Object:** Class-এর একটি নির্দিষ্ট উদাহরণ। যেমন: "আমার Toyota গাড়ি" একটি Object।
- **Attribute/Property:** Object-এর বৈশিষ্ট্য। যেমন: গাড়ির রঙ, মডেল।
- **Method:** Object-এর আচরণ বা কাজ। যেমন: start(), stop(), accelerate()।

---

### 🔷 OOP-এর ৪টি মূল নীতি — বিস্তারিত:

#### ১. Encapsulation (এনক্যাপসুলেশন) — "Data Hiding"

**সংজ্ঞা:** ডেটা (attributes) ও সেই ডেটার উপর কাজ করার মেথড (methods) একটি class-এর ভেতরে আবদ্ধ রাখা। বাইরে থেকে সরাসরি ডেটা পরিবর্তন করা যাবে না।

**Access Modifiers:**
- `private` — শুধু ওই class-এর ভেতরে অ্যাক্সেসযোগ্য
- `protected` — ওই class ও তার subclass-এ
- `public` — সব জায়গা থেকে

```java
class BankAccount {
    private double balance;    // বাইরে থেকে সরাসরি পরিবর্তন করা যাবে না

    public void deposit(double amount) {
        if (amount > 0) balance += amount;
    }

    public void withdraw(double amount) {
        if (amount > 0 && amount <= balance) balance -= amount;
    }

    public double getBalance() {
        return balance;
    }
}
```

**সুবিধা:** ডেটার নিরাপত্তা নিশ্চিত, ভুল ডেটা প্রবেশ রোধ।

---

#### ২. Inheritance (ইনহেরিটেন্স) — "IS-A Relationship"

**সংজ্ঞা:** একটি class (Child/Subclass) আরেকটি class (Parent/Superclass)-এর সমস্ত বৈশিষ্ট্য ও মেথড গ্রহণ করে।

```java
class Animal {
    String name;
    void eat() { System.out.println(name + " is eating"); }
    void breathe() { System.out.println("Breathing..."); }
}

class Dog extends Animal {   // Dog, Animal-কে Inherit করে
    void bark() { System.out.println("Woof!"); }
}

class Cat extends Animal {
    void meow() { System.out.println("Meow!"); }
}
// Dog ও Cat দুটোই Animal-এর eat() ও breathe() পাবে
```

**প্রকারভেদ:**
- **Single:** A → B
- **Multilevel:** A → B → C
- **Hierarchical:** A → B, A → C
- **Multiple:** A + B → C (Java-তে Class-এ নেই, Interface-এ আছে)

**সুবিধা:** কোড পুনর্ব্যবহারযোগ্য, Hierarchical সংগঠন।

---

#### ৩. Polymorphism (পলিমরফিজম) — "একই নাম, ভিন্ন রূপ"

**সংজ্ঞা:** একই নামের মেথড বা অপারেটর ভিন্ন প্রসঙ্গে ভিন্নভাবে কাজ করতে পারে।

**দুই প্রকার:**

**A) Compile-time Polymorphism (Method Overloading):**
```java
class Calculator {
    int add(int a, int b) { return a + b; }          // দুটি int
    double add(double a, double b) { return a + b; }  // দুটি double
    int add(int a, int b, int c) { return a+b+c; }   // তিনটি int
    // একই নাম "add" কিন্তু ভিন্ন parameter
}
```

**B) Runtime Polymorphism (Method Overriding):**
```java
class Shape {
    void draw() { System.out.println("Drawing a shape"); }
}

class Circle extends Shape {
    @Override
    void draw() { System.out.println("Drawing a Circle"); }  // Override করা হলো
}

class Rectangle extends Shape {
    @Override
    void draw() { System.out.println("Drawing a Rectangle"); }
}

// Runtime-এ কোন draw() ডাকা হবে তা Object-এর ধরন অনুযায়ী ঠিক হয়
Shape s = new Circle();
s.draw();  // "Drawing a Circle" — Runtime-এ নির্ধারিত
```

---

#### ৪. Abstraction (অ্যাবস্ট্রাকশন) — "প্রয়োজনীয় তথ্য দেখাও, বাকি লুকাও"

**সংজ্ঞা:** অপ্রয়োজনীয় বিবরণ লুকিয়ে শুধু প্রয়োজনীয় অংশ দেখানো।

```java
// Abstract Class
abstract class Vehicle {
    abstract void startEngine();   // কীভাবে start হবে জানা নেই, শুধু জানি হবে
    void stop() { System.out.println("Stopping..."); }  // সাধারণ মেথড
}

class Car extends Vehicle {
    @Override
    void startEngine() { System.out.println("Car engine started with key"); }
}

class ElectricCar extends Vehicle {
    @Override
    void startEngine() { System.out.println("Electric motor activated silently"); }
}
```

**Interface ব্যবহার:**
```java
interface Printable {
    void print();       // শুধু কী করবে বলে, কীভাবে করবে বলে না
}

class Document implements Printable {
    public void print() { System.out.println("Printing document..."); }
}
```

**পার্থক্য: Abstract Class vs Interface**
| বিষয় | Abstract Class | Interface |
|---|---|---|
| কীওয়ার্ড | `abstract class` | `interface` |
| Implement/Extend | `extends` | `implements` |
| Method | Abstract ও Concrete উভয় | সব Abstract (Java 8+ এ Default Method) |
| Variable | সব ধরন | শুধু `public static final` |
| Multiple Inherit | না | হ্যাঁ |

---

## ৪.২ প্রোগ্রামিং ভাষার প্রকারভেদ — বিস্তারিত

### 🔷 স্তর অনুযায়ী:

| স্তর | প্রকার | বৈশিষ্ট্য | উদাহরণ |
|---|---|---|---|
| **Machine Language (1GL)** | সর্বনিম্ন | শুধু 0 ও 1। CPU সরাসরি বোঝে। মানুষের পক্ষে লেখা প্রায় অসম্ভব। | 01001000 10000101 |
| **Assembly Language (2GL)** | নিম্ন | Mnemonics ব্যবহার (MOV, ADD, JMP)। Assembler দিয়ে Machine Code-এ রূপান্তর। Hardware-নির্ভর। | MOV AX, 5 |
| **High-level Language (3GL)** | উচ্চ | মানুষের ভাষার কাছাকাছি। Compiler/Interpreter দরকার। Hardware-স্বাধীন। | C, Java, Python |
| **4GL** | খুব উচ্চ | SQL-এর মতো Declarative। "কী চাই" বলো, "কীভাবে" সিস্টেম ঠিক করে। | SQL, MATLAB |
| **5GL** | AI-নির্ভর | Constraint-based প্রোগ্রামিং। AI সমাধান খোঁজে। | Prolog, LISP |

---

### 🔷 Compiler vs Interpreter vs Assembler:

| বৈশিষ্ট্য | Compiler | Interpreter | Assembler |
|---|---|---|---|
| **ইনপুট** | High-level source code | High-level source code | Assembly code |
| **আউটপুট** | Machine code (পুরোটা একসাথে) | সরাসরি execute করে | Machine code |
| **অনুবাদের সময়** | আগে একবার | প্রতিটি লাইন চলার সময় | আগে একবার |
| **গতি (রান টাইমে)** | দ্রুত | ধীর | দ্রুত |
| **Error** | সব একসাথে দেখায় | একটি দেখলে থামে | — |
| **উদাহরণ** | GCC (C/C++), javac | Python, Ruby | NASM |

> 📌 **বিশেষ নোট:** Java-তে Hybrid পদ্ধতি — প্রথমে Compiler Bytecode তৈরি করে, তারপর JVM (Interpreter) সেটা চালায়।

---

## ৪.৩ SDLC — সম্পূর্ণ বিস্তারিত

**SDLC = Software Development Life Cycle**
সফটওয়্যার তৈরির পুরো প্রক্রিয়াকে সুনির্দিষ্ট ধাপে ভাগ করার পদ্ধতি।

### 🔷 Waterfall Model — বিস্তারিত:

```
┌─────────────────────────┐
│  1. Requirements        │ ← কী তৈরি করতে হবে তা নথিভুক্ত
└────────────┬────────────┘
             ↓
┌────────────┴────────────┐
│  2. System Design       │ ← Architecture, Database Design
└────────────┬────────────┘
             ↓
┌────────────┴────────────┐
│  3. Implementation      │ ← কোড লেখা
└────────────┬────────────┘
             ↓
┌────────────┴────────────┐
│  4. Testing             │ ← বাগ খোঁজা ও ঠিক করা
└────────────┬────────────┘
             ↓
┌────────────┴────────────┐
│  5. Deployment          │ ← ব্যবহারকারীর কাছে পৌঁছানো
└────────────┬────────────┘
             ↓
┌────────────┴────────────┐
│  6. Maintenance         │ ← আপডেট, বাগ ফিক্স
└─────────────────────────┘
```

**Waterfall-এর সমস্যা:** একটি ধাপ শেষ না হলে পরেরটি শুরু হয় না। পরিবর্তন করা কঠিন।

---

### 🔷 Agile Model — বিস্তারিত:

Agile হলো ইটারেটিভ (পুনরাবৃত্তিমূলক) পদ্ধতি। প্রতিটি **Sprint** (২-৪ সপ্তাহ) একটি কার্যকর সফটওয়্যার ইনক্রিমেন্ট তৈরি করে।

```
Sprint 1 → Sprint 2 → Sprint 3 → ... → সম্পূর্ণ সফটওয়্যার
(প্রতিটি Sprint-এ: Plan → Design → Code → Test → Review)
```

**Agile Manifesto-এর মূল্যবোধ:**
1. ব্যক্তি ও মিথস্ক্রিয়া > প্রক্রিয়া ও সরঞ্জাম
2. কার্যকর সফটওয়্যার > ব্যাপক ডকুমেন্টেশন
3. গ্রাহক সহযোগিতা > চুক্তি আলোচনা
4. পরিবর্তনে সাড়া দেওয়া > পরিকল্পনা অনুসরণ

### 🔷 Waterfall vs Agile:

| বৈশিষ্ট্য | Waterfall | Agile |
|---|---|---|
| **পদ্ধতি** | Sequential (ধাপে ধাপে) | Iterative (চক্রাকার) |
| **নমনীয়তা** | কম | বেশি |
| **Requirement** | শুরুতেই সব নির্ধারিত | পরিবর্তনযোগ্য |
| **গ্রাহক সম্পৃক্ততা** | শুরু ও শেষে | প্রতিটি Sprint-এ |
| **ডেলিভারি** | শেষে একবার | প্রতিটি Sprint-এ |
| **উপযুক্ত** | স্থির requirement | পরিবর্তনশীল requirement |
| **ঝুঁকি** | বেশি (শেষে সমস্যা দেখা দিলে) | কম (তাড়াতাড়ি সমস্যা ধরা পড়ে) |

### 🔷 অন্যান্য SDLC Models:
- **Spiral Model:** Waterfall + Risk Analysis (ঝুঁকি মূল্যায়ন)
- **V-Model:** Waterfall-এ প্রতিটি ধাপের সাথে Test ধাপ যুক্ত
- **Prototype Model:** আগে ছোট মডেল তৈরি করে গ্রাহককে দেখানো
- **RAD (Rapid Application Development):** দ্রুত উন্নয়ন, পুনর্ব্যবহারযোগ্য Component

---

## ৪.৪ Application Framework — বিস্তারিত

**📌 BB AME 2019 পরীক্ষায় এসেছিল!**

### 🔷 Framework কী?
Framework হলো পুনর্ব্যবহারযোগ্য কোড, লাইব্রেরি ও টুলের সমষ্টি যা অ্যাপ্লিকেশন তৈরির ভিত্তি হিসেবে কাজ করে।

### 🔷 জনপ্রিয় Framework:

| ভাষা | Framework | ব্যবহার |
|---|---|---|
| Python | Django, Flask | Web Backend |
| JavaScript | React, Angular, Vue | Web Frontend |
| JavaScript | Node.js, Express | Web Backend |
| Java | Spring Boot | Enterprise Web |
| PHP | Laravel, CodeIgniter | Web Backend |
| C# | ASP.NET | Microsoft Web |

### 🔷 Framework-এর সুবিধা:
1. **Code Reusability:** চাকা পুনরায় আবিষ্কার করতে হয় না — তৈরি Component ব্যবহার করা যায়
2. **MVC Pattern:** Model-View-Controller আর্কিটেকচার দেয় — কোড সুসংগঠিত থাকে
3. **Security:** Built-in নিরাপত্তা (SQL Injection, XSS রোধ) থাকে
4. **Community Support:** বড় সম্প্রদায় — সমস্যায় সাহায্য পাওয়া যায়
5. **Testing সহজ:** Built-in Testing টুল থাকে
6. **Maintainability:** কোড আপডেট ও রক্ষণাবেক্ষণ সহজ

### 🔷 Framework-এর অসুবিধা:
1. **শেখার সময়:** Framework নিজেই শিখতে সময় লাগে
2. **Flexibility হ্রাস:** Framework-এর নিয়ম মেনে চলতে হয়
3. **Performance:** Extra abstraction-এ কিছুটা গতি কমতে পারে
4. **Over-engineering:** ছোট প্রজেক্টের জন্য অতিরিক্ত জটিলতা

---

---

# ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
# অধ্যায় ৫: অপারেটিং সিস্টেম
### 🟡 মাঝারি গুরুত্ব (~১৫%)
# ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

---

## ৫.১ OS মৌলিক ধারণা — বিস্তারিত

### 🔷 Operating System কী?
OS হলো একটি সিস্টেম সফটওয়্যার যা হার্ডওয়ার ও ব্যবহারকারীর মধ্যে মধ্যস্থতাকারী হিসেবে কাজ করে। এটি হার্ডওয়ার সম্পদ পরিচালনা করে এবং অন্যান্য সফটওয়্যার চালানোর পরিবেশ তৈরি করে।

**OS ছাড়া:** সরাসরি Machine Language-এ হার্ডওয়ার নিয়ন্ত্রণ করতে হতো।

### 🔷 OS-এর প্রধান কাজ — বিস্তারিত:

| কাজ | বিবরণ |
|---|---|
| **Process Management** | প্রোগ্রাম চালানো, থামানো, CPU সময় ভাগ করা |
| **Memory Management** | RAM বরাদ্দ ও মুক্তি দেওয়া, Virtual Memory পরিচালনা |
| **File System Management** | ফাইল তৈরি, মুছা, সংগঠিত করা, ডিরেক্টরি পরিচালনা |
| **I/O Device Management** | Keyboard, Mouse, Printer নিয়ন্ত্রণ করা |
| **Security** | ব্যবহারকারী Authentication, Authorization, Data Protection |
| **Error Detection** | Hardware ও Software error শনাক্ত ও সমাধান |
| **Job Scheduling** | কোন প্রোগ্রাম কখন CPU পাবে তা নির্ধারণ |
| **Networking** | নেটওয়ার্ক সংযোগ পরিচালনা |

### 🔷 OS প্রকারভেদ:

| প্রকার | বৈশিষ্ট্য | উদাহরণ |
|---|---|---|
| **Batch OS** | User সরাসরি কথা বলে না। Jobs batch-এ জমা দেয়, OS একে একে চালায়। | IBM OS/360 |
| **Time-sharing OS** | একাধিক user একসাথে কাজ করে। CPU সময়কে ভাগ করে দেওয়া হয়। | UNIX, Linux |
| **Real-time OS** | নির্দিষ্ট সময়ের মধ্যে (deadline) response দিতে হয়। | VxWorks, FreeRTOS (রকেট, মেডিকেল) |
| **Distributed OS** | একাধিক কম্পিউটার একটি OS-এর অধীনে একসাথে কাজ করে। | Amoeba, Chorus |
| **Embedded OS** | বিশেষ ডিভাইসের জন্য তৈরি, সীমিত সম্পদে কাজ করে। | Android, iOS, Raspbian |
| **Network OS** | নেটওয়ার্কে সংযুক্ত ডিভাইস পরিচালনা। | Novell NetWare, Windows Server |

---

## ৫.২ Kernel — বিস্তারিত

**📌 BB AME 2019 পরীক্ষায় এসেছিল!**

### 🔷 Kernel কী?
Kernel হলো OS-এর মূল/কেন্দ্রীয় অংশ। এটি সবসময় RAM-এ থাকে এবং হার্ডওয়ার ও সফটওয়্যারের মধ্যে সরাসরি যোগাযোগ করে।

### 🔷 Microkernel vs Monolithic Kernel:

| বৈশিষ্ট্য | Microkernel | Monolithic Kernel |
|---|---|---|
| **আকার** | ছোট — শুধু অত্যন্ত প্রয়োজনীয় সেবা Kernel-এ | বড় — সব সেবা Kernel-এ |
| **Kernel-এ কী থাকে** | IPC, Memory Management, Scheduling | + File System, Device Driver, Network |
| **বাকি সেবা** | User Space-এ আলাদা প্রক্রিয়া হিসেবে চলে | Kernel Space-এ চলে |
| **নিরাপত্তা** | বেশি — একটি অংশ ক্র্যাশ করলে পুরো OS পড়ে না | কম — একটি ক্র্যাশ পুরো সিস্টেম নামাতে পারে |
| **গতি** | ধীর — User-Kernel Space যোগাযোগে overhead | দ্রুত — সব একসাথে Kernel-এ |
| **পরিবর্তনযোগ্যতা** | সহজ — Module আলাদা করা যায় | কঠিন |
| **উদাহরণ** | MINIX, QNX, L4, macOS (Mach-based) | Linux, UNIX, FreeBSD |
| **Windows NT** | Hybrid (Microkernel + Monolithic উভয়) | — |

### 🔷 Windows NT I/O Manager-এর Sub-components:
1. **Network Redirector/Server** — নেটওয়ার্ক ফাইল অ্যাক্সেস পরিচালনা
2. **Cache Manager** — ডেটা Cache পরিচালনা
3. **File Systems** — FAT, NTFS ফাইল সিস্টেম পরিচালনা
4. **Network Driver Interface** — নেটওয়ার্ক কার্ড ড্রাইভার
5. **Device Driver** — Hardware Driver পরিচালনা

---

## ৫.৩ Process Management — বিস্তারিত

### 🔷 Process vs Program:
- **Program:** ডিস্কে সংরক্ষিত নিষ্ক্রিয় কোড
- **Process:** RAM-এ লোড হয়ে চলমান প্রোগ্রাম

### 🔷 Process State Diagram:

```
         ┌─────────────┐
         │     NEW     │ ← প্রোগ্রাম শুরু হচ্ছে
         └──────┬──────┘
                │ (Admitted)
         ┌──────▼──────┐
    ┌────│    READY    │◀──────────────────┐
    │    └──────┬──────┘                   │
    │           │ (Dispatched / CPU পেল)   │
    │    ┌──────▼──────┐                   │
    │    │   RUNNING   │ ── (I/O চাই) ──▶ │
    │    └──────┬──────┘  ┌─────────────┐  │
    │           │          │   WAITING   │──┘
    │    (Exit) │          └─────────────┘
    │    ┌──────▼──────┐   (I/O শেষ)
    │    │ TERMINATED  │
    │    └─────────────┘
    │                       (Preempted / সময় শেষ)
    └──────────────────────────────────────────▶ READY
```

| অবস্থা | বর্ণনা |
|---|---|
| **New** | Process তৈরি হচ্ছে, RAM-এ লোড হচ্ছে |
| **Ready** | CPU পাওয়ার জন্য Queue-এ অপেক্ষা করছে |
| **Running** | CPU-এ বর্তমানে চলছে (execute হচ্ছে) |
| **Waiting/Blocked** | I/O অপারেশন বা Event-এর জন্য অপেক্ষা করছে |
| **Terminated** | Process সম্পূর্ণ হয়েছে বা বাতিল হয়েছে |

### 🔷 PCB (Process Control Block):
প্রতিটি Process-এর সব তথ্য OS যে ডেটা স্ট্রাকচারে রাখে:
- Process ID (PID)
- Process State
- Program Counter
- CPU Registers
- Memory Information
- I/O Status

---

## ৫.৪ CPU Scheduling Algorithms — বিস্তারিত

### 🔷 ৪টি প্রধান Algorithm:

#### ১. FCFS — First Come First Serve
- **নিয়ম:** যে আগে আসে সে আগে CPU পায়
- **সমস্যা:** Convoy Effect — ছোট process দীর্ঘক্ষণ অপেক্ষা করে

**উদাহরণ:**
```
Process:  P1(Burst=24), P2(Burst=3), P3(Burst=3)
Gantt:  |── P1 ──|P2|P3|
Time:   0        24  27  30
Average Waiting Time = (0 + 24 + 27) / 3 = 17 ms  ← বেশি!
```

#### ২. SJF — Shortest Job First
- **নিয়ম:** সবচেয়ে ছোট Burst Time-এর process আগে
- **সমস্যা:** Starvation — বড় process কখনো CPU নাও পেতে পারে

**উদাহরণ:**
```
Process:  P2(Burst=3), P3(Burst=3), P1(Burst=24)
Gantt:  |P2|P3|── P1 ──|
Time:   0   3   6       30
Average Waiting Time = (6 + 0 + 3) / 3 = 3 ms  ← অনেক কম!
```

#### ৩. Round Robin (RR)
- **নিয়ম:** প্রতিটি process কে Time Quantum (TQ) পরিমাণ সময় দেওয়া হয়, তারপর পরেরটি
- **সুবিধা:** Fair, Time-sharing-এ আদর্শ
- **সমস্যা:** TQ বড় হলে FCFS-এর মতো; ছোট হলে Context Switch বেশি

#### ৪. Priority Scheduling
- **নিয়ম:** উচ্চ Priority-এর process আগে CPU পায়
- **সমস্যা:** Starvation — কম Priority-এর process অনেক অপেক্ষা করে
- **সমাধান:** Aging — অপেক্ষার সময় বাড়ার সাথে Priority বাড়ে

| Algorithm | Preemptive? | Starvation? | Overhead | উপযুক্ত |
|---|---|---|---|---|
| FCFS | না | না | কম | Batch |
| SJF | না (Non-preemptive) | হ্যাঁ | কম | Batch |
| SRTF | হ্যাঁ | হ্যাঁ | বেশি | — |
| RR | হ্যাঁ | না | বেশি | Time-sharing |
| Priority | উভয় | হ্যাঁ | মাঝারি | Real-time |

---

## ৫.৫ Deadlock — বিস্তারিত

### 🔷 Deadlock কী?
Deadlock হলো এমন পরিস্থিতি যেখানে দুই বা ততোধিক Process একে অপরের ধরে রাখা Resource-এর জন্য অনির্দিষ্টকাল অপেক্ষা করছে।

**উদাহরণ:** Process A ধরে আছে Printer, চাইছে Scanner।
Process B ধরে আছে Scanner, চাইছে Printer।
→ উভয়ই অপেক্ষা করছে, কেউ এগোতে পারছে না।

### 🔷 Deadlock-এর ৪টি শর্ত (Coffman Conditions):
1. **Mutual Exclusion:** Resource একসাথে শুধু একটি Process ব্যবহার করতে পারে
2. **Hold and Wait:** একটি Resource ধরে আরেকটির জন্য অপেক্ষা করছে
3. **No Preemption:** Resource জোর করে কেড়ে নেওয়া যাবে না
4. **Circular Wait:** P1 → P2 → P3 → P1 এভাবে বৃত্তাকার নির্ভরশীলতা

> সব ৪টি শর্ত একসাথে পূরণ হলেই Deadlock হয়।

### 🔷 Deadlock মোকাবেলা:
- **Prevention:** ৪টি শর্তের যেকোনো একটি ভেঙে দাও (আগেভাগে)
- **Avoidance:** Banker's Algorithm — নিরাপদ অবস্থায় Resource দাও
- **Detection & Recovery:** Deadlock হতে দাও, পরে শনাক্ত করে Process Kill বা Resource নাও
- **Ignorance:** (Ostrich Algorithm) Deadlock বিরল হলে উপেক্ষা করো (Windows/Linux-এ ব্যবহৃত)

---

## ৫.৬ Memory Management — বিস্তারিত

### 🔷 Virtual Memory:
Physical RAM-এর চেয়ে বড় প্রোগ্রাম চালানোর কৌশল। HDD/SSD-এর একটি অংশ (Swap Space/Page File) RAM হিসেবে ব্যবহার করা হয়।

```
┌─────────────────┐
│   Program       │ (মোট আকার: 1 GB)
│   Virtual       │
│   Address Space │
└────────┬────────┘
         │ (OS পরিচালনা করে)
    ┌────┴───────────────────┐
    │         │              │
┌───▼───┐  ┌─▼──────────┐   
│  RAM  │  │ HDD/SSD    │   
│ (4GB) │  │ Swap Space │   
└───────┘  └────────────┘   
```

### 🔷 Paging:
- Memory-কে সমান আকারের **Page (Frame)**-এ ভাগ করা
- Physical Memory = **Frame**
- Logical Memory = **Page**
- **Page Table:** Page থেকে Frame-এ mapping রাখে
- **Page Fault:** দরকারি Page RAM-এ না থাকলে HDD থেকে আনতে হয়

### 🔷 Segmentation:
- Memory-কে অর্থপূর্ণ **Segment**-এ ভাগ করা (Code, Data, Stack আলাদা)
- প্রতিটি Segment ভিন্ন আকারের

### 🔷 Page Replacement Algorithms:
| Algorithm | নিয়ম |
|---|---|
| **FIFO** | সবচেয়ে পুরনো Page বের করো |
| **LRU** | সবচেয়ে বেশি দিন ব্যবহার হয়নি সেটি বের করো (সর্বোত্তম) |
| **Optimal** | ভবিষ্যতে সবচেয়ে দেরিতে দরকার হবে সেটি বের করো |

---

---

# ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
# অধ্যায় ৬: ডেটা স্ট্রাকচার ও অ্যালগরিদম
### 🟡 মাঝারি গুরুত্ব (~১২%)
# ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

---

## ৬.১ মৌলিক ডেটা স্ট্রাকচার — বিস্তারিত

### 🔷 Array (অ্যারে):
- একই ধরনের ডেটার **ক্রমানুসারে** সংগ্রহ
- **Index** দিয়ে সরাসরি যেকোনো element-এ অ্যাক্সেস
- **সুবিধা:** দ্রুত অ্যাক্সেস — O(1)
- **অসুবিধা:** আকার নির্দিষ্ট, মাঝখানে যোগ/বাদ দিতে সব সরাতে হয় — O(n)

```
Index: [0]  [1]  [2]  [3]  [4]
Data:  [10] [20] [30] [40] [50]
        ↑
    arr[0] = 10 → O(1) তে অ্যাক্সেস
```

### 🔷 Linked List:
প্রতিটি **Node**-এ ডেটা ও পরের Node-এর **Pointer** থাকে।

```
[Data|Next]→[Data|Next]→[Data|Next]→NULL
   10           20           30
```

| প্রকার | বিবরণ |
|---|---|
| **Singly Linked** | প্রতিটি Node-এ শুধু next pointer |
| **Doubly Linked** | প্রতিটি Node-এ next ও previous pointer |
| **Circular Linked** | শেষ Node-এর next প্রথম Node-কে দেখায় |

**Array vs Linked List:**
| বিষয় | Array | Linked List |
|---|---|---|
| Access | O(1) | O(n) |
| Search | O(n) | O(n) |
| Insert/Delete শেষে | O(1) | O(1) |
| Insert/Delete মাঝে | O(n) | O(1) (pointer জানলে) |
| মেমোরি | Continuous | Scattered |

---

### 🔷 Stack (স্ট্যাক) — LIFO:
**Last In First Out** — যে শেষে ঢোকে সে প্রথমে বের হয়।

```
        ┌─────┐  ← TOP
        │  5  │  ← সবার শেষে Push হয়েছে, প্রথমে Pop হবে
        ├─────┤
        │  4  │
        ├─────┤
        │  3  │
        ├─────┤
        │  2  │
        ├─────┤
        │  1  │  ← সবার আগে Push হয়েছে, সবার শেষে Pop হবে
        └─────┘
```

**Operations:**
- `push(x)` — Stack-এ ঢোকানো
- `pop()` — উপর থেকে বের করা
- `peek()/top()` — উপরেরটি না সরিয়ে দেখা
- `isEmpty()` — খালি কিনা চেক

**Real-life Applications:**
- Function call stack (Recursion)
- Expression evaluation (postfix/prefix)
- Undo/Redo (Ctrl+Z)
- Browser back button
- Balanced Parentheses check

---

### 🔷 Queue (কিউ) — FIFO:
**First In First Out** — যে প্রথমে ঢোকে সে প্রথমে বের হয়।

```
REAR → [5][4][3][2][1] → FRONT
         ↑                  ↑
      এখানে ঢোকে       এখানে বের হয়
    (Enqueue)           (Dequeue)
```

**প্রকারভেদ:**
- **Simple Queue:** সাধারণ FIFO
- **Circular Queue:** শেষ position পূর্ণ হলে শুরুতে ফিরে যায়
- **Priority Queue:** Priority অনুযায়ী বের হয়
- **Deque (Double-ended Queue):** উভয় প্রান্ত থেকে ঢোকানো ও বের করা যায়

**Real-life Applications:**
- Print queue (প্রিন্টারের অপেক্ষা তালিকা)
- CPU Scheduling (Round Robin)
- BFS traversal
- Call center queue

---

### 🔷 Tree (ট্রি):
হায়ারার্কিক্যাল ডেটা স্ট্রাকচার। একটি Root Node থেকে শুরু হয়ে শাখা-প্রশাখায় ছড়িয়ে যায়।

**গুরুত্বপূর্ণ পরিভাষা:**
- **Root:** সর্বোচ্চ Node (কোনো parent নেই)
- **Leaf:** সর্বনিম্ন Node (কোনো child নেই)
- **Height:** Root থেকে সবচেয়ে নিচের Leaf পর্যন্ত দূরত্ব
- **Depth:** Root থেকে একটি Node-এর দূরত্ব

**Binary Tree:** প্রতিটি Node-এ সর্বোচ্চ ২টি child।

---

## ৬.২ Tree Traversal — বিস্তারিত উদাহরণ

```
           1        ← Root
          / \
         2   3
        / \
       4   5
```

| Traversal | ক্রম | পদ্ধতি | ফলাফল |
|---|---|---|---|
| **Inorder** | Left → Root → Right | বাম গাছ → Root → ডান গাছ | **4, 2, 5, 1, 3** |
| **Preorder** | Root → Left → Right | Root → বাম গাছ → ডান গাছ | **1, 2, 4, 5, 3** |
| **Postorder** | Left → Right → Root | বাম গাছ → ডান গাছ → Root | **4, 5, 2, 3, 1** |
| **Level Order (BFS)** | স্তর অনুযায়ী | Queue ব্যবহার | **1, 2, 3, 4, 5** |

> 📌 **মনে রাখো:** BST (Binary Search Tree)-এর Inorder Traversal সর্বদা ক্রমানুসারে (sorted) ফলাফল দেয়।

---

## ৬.৩ Sorting Algorithms — সম্পূর্ণ বিস্তারিত

### 🔷 Bubble Sort:
প্রতিটি pass-এ পাশাপাশি দুটি element তুলনা করে, বড়টি পিছনে পাঠাও।

```
Pass 1: [64, 34, 25, 12, 22, 11, 90]
Step:   [34, 25, 12, 22, 11, 64, 90]  ← 64 বুদবুদের মতো উপরে উঠলো
Pass 2: [25, 12, 22, 11, 34, 64, 90]
...
```

### 🔷 Selection Sort:
প্রতিটি pass-এ সবচেয়ে ছোটটি খুঁজে সামনে রাখো।

### 🔷 Insertion Sort:
প্রতিটি element-কে তার সঠিক অবস্থানে সন্নিবেশ করো (তাসের খেলার মতো)।

### 🔷 Merge Sort:
Divide & Conquer — অর্ধেক ভাগ করো, প্রতিটি অর্ধ sort করো, তারপর merge করো।

### 🔷 Quick Sort:
Divide & Conquer — Pivot নির্বাচন করো, ছোটগুলো বামে বড়গুলো ডানে।

### 🔷 Time Complexity তুলনা:

| Algorithm | Best Case | Average Case | Worst Case | Space | Stable? |
|---|---|---|---|---|---|
| **Bubble Sort** | O(n) | O(n²) | O(n²) | O(1) | হ্যাঁ |
| **Selection Sort** | O(n²) | O(n²) | O(n²) | O(1) | না |
| **Insertion Sort** | O(n) | O(n²) | O(n²) | O(1) | হ্যাঁ |
| **Merge Sort** | O(n log n) | O(n log n) | **O(n log n)** | O(n) | হ্যাঁ |
| **Quick Sort** | O(n log n) | O(n log n) | O(n²) | O(log n) | না |
| **Heap Sort** | O(n log n) | O(n log n) | O(n log n) | O(1) | না |

> 📌 **গুরুত্বপূর্ণ:** Merge Sort সবসময় O(n log n) — Worst Case-ও। পরীক্ষায় বারবার আসে!
> Stable Sort = সমান মানের element-এর আপেক্ষিক ক্রম অপরিবর্তিত থাকে।

---

## ৬.৪ Searching Algorithms:

### 🔷 Linear Search:
- প্রতিটি element পরীক্ষা করো
- Time Complexity: O(n)
- Sort করা দরকার নেই

### 🔷 Binary Search:
- **শর্ত:** Array অবশ্যই sorted থাকতে হবে
- মাঝের element-এর সাথে তুলনা করো, অর্ধেক বাদ দাও
- Time Complexity: O(log n)

```
Array: [1, 3, 5, 7, 9, 11, 13, 15] খুঁজছি: 7
Step 1: Middle = 7 (index 3)? হ্যাঁ! পাওয়া গেছে।
```

---

## ৬.৫ Big-O Notation — বিস্তারিত

অ্যালগরিদমের **সময় ও স্থান জটিলতা** বোঝানোর পদ্ধতি।

| Notation | নাম | উদাহরণ | ব্যাখ্যা |
|---|---|---|---|
| **O(1)** | Constant | Array index access | Input বাড়লেও সময় একই |
| **O(log n)** | Logarithmic | Binary Search | Input দ্বিগুণ হলে ১ ধাপ বাড়ে |
| **O(n)** | Linear | Linear Search | Input-এর সমানুপাতে সময় বাড়ে |
| **O(n log n)** | Linearithmic | Merge Sort, Quick Sort | — |
| **O(n²)** | Quadratic | Bubble Sort, Selection Sort | Nested loop |
| **O(2ⁿ)** | Exponential | Fibonacci (Recursive) | Input একটু বাড়লে বিশাল সময় |
| **O(n!)** | Factorial | Traveling Salesman | সবচেয়ে ধীর |

**গতির ক্রম (দ্রুত থেকে ধীর):**
```
O(1) < O(log n) < O(n) < O(n log n) < O(n²) < O(2ⁿ) < O(n!)
```

---

---

# ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
# অধ্যায় ৭: সাইবার সিকিউরিটি
### 🟡 মাঝারি গুরুত্ব (~১০%)
# ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

---

## ৭.১ Malware — সম্পূর্ণ বিস্তারিত

**Malware = Malicious Software** — ক্ষতিকর সফটওয়্যার।

| প্রকার | বৈশিষ্ট্য | ছড়ানোর পদ্ধতি | ক্ষতি |
|---|---|---|---|
| **Virus** | Host ফাইলের সাথে যুক্ত হয়। সেই ফাইল চালালে ছড়ায়। | ফাইল শেয়ার, Email attachment | ফাইল নষ্ট করা, ডেটা মুছা |
| **Worm** | নিজে নিজে নেটওয়ার্কে ছড়ায়, Host দরকার নেই | নেটওয়ার্ক ভালনারেবিলিটি | ব্যান্ডউইথ খরচ, সিস্টেম স্লো |
| **Trojan Horse** | বৈধ সফটওয়্যার সেজে ক্ষতি করে। নিজে ছড়ায় না। | ডাউনলোড, ফিশিং | Backdoor তৈরি, ডেটা চুরি |
| **Ransomware** | ফাইল এনক্রিপ্ট করে মুক্তিপণ (Bitcoin) দাবি করে | Email, Exploit | ফাইল অ্যাক্সেস করতে পারা যায় না |
| **Spyware** | ব্যবহারকারীর অজান্তে তথ্য সংগ্রহ করে | Drive-by Download | পাসওয়ার্ড, ক্রেডিট কার্ড চুরি |
| **Adware** | অবাঞ্ছিত বিজ্ঞাপন দেখায় | Freeware-এর সাথে | ব্রাউজার Redirect, স্লো সিস্টেম |
| **Rootkit** | OS-এর গভীরে লুকিয়ে থেকে Admin অধিকার নেয় | Exploit | অদৃশ্য থেকে সিস্টেম নিয়ন্ত্রণ |
| **Keylogger** | কীবোর্ডের প্রতিটি কীস্ট্রোক রেকর্ড করে | Trojan-এর মাধ্যমে | পাসওয়ার্ড ও গোপন তথ্য চুরি |
| **Botnet** | অনেক কম্পিউটার একটি নেটওয়ার্কে নিয়ন্ত্রণে নেওয়া | Worm | DDoS Attack |

---

## ৭.২ Attack — সম্পূর্ণ বিস্তারিত

| Attack | সম্পূর্ণ ব্যাখ্যা | প্রতিরোধ |
|---|---|---|
| **Phishing** | ভুয়া ওয়েবসাইট বা ইমেইলে বিশ্বাসযোগ্য প্রতিষ্ঠান (ব্যাংক, Google) সেজে পাসওয়ার্ড চুরি | URL যাচাই, 2FA, সচেতনতা |
| **Spear Phishing** | নির্দিষ্ট ব্যক্তি/প্রতিষ্ঠানকে লক্ষ্য করে tailored ফিশিং | — |
| **DoS** | একটি উৎস থেকে প্রচুর request পাঠিয়ে সার্ভার অকেজো করা | Firewall, Rate Limiting |
| **DDoS** | হাজারো কম্পিউটার (Botnet) থেকে একসাথে আক্রমণ — প্রতিরোধ কঠিন | CDN, Traffic Filtering |
| **Man-in-the-Middle (MitM)** | দুটি পক্ষের যোগাযোগের মাঝখানে ঢুকে ডেটা পড়া বা পরিবর্তন | HTTPS, Certificate Pinning |
| **SQL Injection** | ইনপুট ফিল্ডে ক্ষতিকর SQL কোড ঢুকিয়ে ডেটাবেজ নিয়ন্ত্রণ | Prepared Statement, Input Validation |
| **XSS** | ওয়েবসাইটে ক্ষতিকর JavaScript inject করে অন্য ব্যবহারকারীর ক্ষতি | Output Encoding, CSP |
| **Brute Force** | সব সম্ভাব্য পাসওয়ার্ড একে একে চেষ্টা করা | Account Lockout, Strong Password |
| **Dictionary Attack** | সাধারণ পাসওয়ার্ড তালিকা দিয়ে চেষ্টা | Salted Hashing |
| **Zero-day Attack** | অজানা ভালনারেবিলিটি ব্যবহার করে আক্রমণ | — (প্যাচ আসার আগেই আক্রমণ) |
| **Social Engineering** | প্রযুক্তির বদলে মানুষকে প্রতারণা করে তথ্য নেওয়া | সচেতনতা ও প্রশিক্ষণ |

---

## ৭.৩ Encryption — সম্পূর্ণ বিস্তারিত

### 🔷 মূল ধারণা:
- **Plaintext:** মূল পাঠযোগ্য ডেটা
- **Ciphertext:** এনক্রিপ্টেড (অপাঠযোগ্য) ডেটা
- **Key:** এনক্রিপশন/ডিক্রিপশনের গোপন চাবি
- **Encryption:** Plaintext → Ciphertext
- **Decryption:** Ciphertext → Plaintext

---

### 🔷 Symmetric Encryption (প্রতিসম এনক্রিপশন):

একই Key দিয়ে **Encrypt ও Decrypt** উভয়ই করা হয়।

```
Sender:  Plaintext → [Encrypt with Secret Key] → Ciphertext → পাঠানো হলো
Receiver: Ciphertext → [Decrypt with Same Secret Key] → Plaintext
```

| Algorithm | Key Size | বৈশিষ্ট্য |
|---|---|---|
| **AES** (Advanced Encryption Standard) | 128/192/256-bit | বর্তমানে সবচেয়ে নিরাপদ ও ব্যাপকভাবে ব্যবহৃত |
| **DES** (Data Encryption Standard) | 56-bit | পুরনো, দুর্বল — ব্যবহার করা উচিত নয় |
| **3DES** (Triple DES) | 112/168-bit | DES তিনবার — DES-এর চেয়ে নিরাপদ কিন্তু ধীর |
| **RC4** | Variable | Stream Cipher, WEP-এ ব্যবহৃত (দুর্বল) |

**সুবিধা:** দ্রুত।  
**অসুবিধা:** Key নিরাপদে শেয়ার করা চ্যালেঞ্জ।

---

### 🔷 Asymmetric Encryption (অপ্রতিসম এনক্রিপশন):

**Public Key** দিয়ে Encrypt, **Private Key** দিয়ে Decrypt।

```
Receiver-এর Public Key (সবার কাছে প্রকাশ্য)
         ↓
Sender:  Plaintext → [Encrypt with Receiver's Public Key] → Ciphertext
         ↓
Receiver: Ciphertext → [Decrypt with Own Private Key] → Plaintext
```

| Algorithm | Key Size | ব্যবহার |
|---|---|---|
| **RSA** | 2048/4096-bit | HTTPS, Email encryption, Digital Signature |
| **ECC** (Elliptic Curve) | 256-bit | Mobile, IoT (RSA-এর চেয়ে ছোট key-এ সমান নিরাপত্তা) |
| **DSA** | 1024-3072-bit | Digital Signature |

**সুবিধা:** Key শেয়ারের সমস্যা নেই।  
**অসুবিধা:** ধীর।

> 📌 **HTTPS-এ উভয় ব্যবহার:** প্রথমে Asymmetric দিয়ে Symmetric Key বিনিময় হয়, তারপর Symmetric দিয়ে ডেটা এনক্রিপ্ট হয় (দ্রুততার জন্য)।

---

### 🔷 Hash Function:
- **একমুখী:** Hash থেকে মূল ডেটায় ফিরে যাওয়া যায় না
- **নির্ধারক:** একই Input সবসময় একই Hash দেয়
- **ব্যবহার:** পাসওয়ার্ড সংরক্ষণ, ডেটা Integrity যাচাই, Digital Signature

| Algorithm | Output Size | বর্তমান অবস্থা |
|---|---|---|
| **MD5** | 128-bit | দুর্বল, Collision পাওয়া গেছে |
| **SHA-1** | 160-bit | দুর্বল, ব্যবহার বন্ধ |
| **SHA-256** | 256-bit | নিরাপদ, ব্যাপকভাবে ব্যবহৃত |
| **SHA-3** | Variable | সর্বশেষ, অত্যন্ত নিরাপদ |
| **bcrypt** | — | পাসওয়ার্ড হ্যাশিং-এ আদর্শ |

**Salt কী?** পাসওয়ার্ড হ্যাশ করার আগে একটি র‍্যান্ডম মান যোগ করা — Dictionary Attack রোধ করে।

---

### 🔷 SSL/TLS:
| বিষয় | SSL | TLS |
|---|---|---|
| **পূর্ণনাম** | Secure Sockets Layer | Transport Layer Security |
| **অবস্থা** | পুরনো, দুর্বল (SSL 3.0 বন্ধ) | বর্তমান মান (TLS 1.2/1.3) |
| **ব্যবহার** | HTTPS, FTPS, SMTPS | HTTPS (HTTPS = HTTP + TLS) |

**SSL/TLS Handshake:**
1. Client → Server: "আমি কথা বলতে চাই, এই cipher list"
2. Server → Client: Certificate পাঠায় (Public Key সহ)
3. Client: Certificate যাচাই করে (CA দিয়ে)
4. উভয়ে Session Key তৈরি করে
5. এনক্রিপ্টেড যোগাযোগ শুরু

---

## ৭.৪ Cloud Computing — বিস্তারিত

### 🔷 Cloud Computing কী?
Internet-এর মাধ্যমে Computing সম্পদ (Server, Storage, Database, Software) ভাড়ায় ব্যবহার করার পদ্ধতি।

**বৈশিষ্ট্য (NIST সংজ্ঞা):**
- **On-demand Self-service:** প্রয়োজনমতো নিজেই নেওয়া যায়
- **Broad Network Access:** যেকোনো ডিভাইস থেকে অ্যাক্সেস
- **Resource Pooling:** সম্পদ ভাগ করে নেওয়া
- **Rapid Elasticity:** দ্রুত বাড়ানো-কমানো
- **Measured Service:** ব্যবহার অনুযায়ী পেমেন্ট (Pay-as-you-go)

---

### 🔷 Service Model — বিস্তারিত:

| মডেল | পূর্ণরূপ | ব্যবহারকারী যা পায় | ব্যবহারকারী যা পরিচালনা করে | উদাহরণ |
|---|---|---|---|---|
| **IaaS** | Infrastructure as a Service | Virtual Machine, Storage, Networking | OS, Runtime, Application | AWS EC2, Google Compute Engine, Azure VM |
| **PaaS** | Platform as a Service | OS + Runtime + Development Tools | শুধু Application ও Data | Google App Engine, Heroku, Azure App Service |
| **SaaS** | Software as a Service | সম্পূর্ণ অ্যাপ্লিকেশন | কিছুই না | Gmail, Microsoft 365, Salesforce, Zoom |

**উপমা:**
- **IaaS** = জমি ভাড়া (নিজে বাড়ি বানাও)
- **PaaS** = ফার্নিচারসহ ফ্ল্যাট ভাড়া (শুধু থাকো)
- **SaaS** = হোটেলে থাকা (সব সুবিধা দেওয়া আছে)

---

### 🔷 Deployment Model:

| মডেল | বৈশিষ্ট্য | উপযুক্ত |
|---|---|---|
| **Public Cloud** | সবার জন্য উন্মুক্ত, Provider পরিচালনা করে | Startup, ছোট প্রতিষ্ঠান |
| **Private Cloud** | শুধু একটি Organization-এর জন্য | ব্যাংক, সরকার (নিরাপত্তা গুরুত্বপূর্ণ) |
| **Hybrid Cloud** | Public ও Private-এর মিশ্রণ | বড় প্রতিষ্ঠান |
| **Community Cloud** | একই খাতের একাধিক প্রতিষ্ঠান ভাগ করে | সরকারি বিভাগ |

---

## ৭.৫ বাংলাদেশের সাইবার আইন — সম্পূর্ণ

| আইন | বছর | মূল বিষয় |
|---|---|---|
| **ICT Act** | ২০০৬ | বাংলাদেশের প্রথম IT আইন। Section 57: অনলাইনে মানহানি, ধর্মীয় অনুভূতিতে আঘাত। |
| **Digital Security Act (DSA)** | ২০১৮ | ICT Act-এর Section 57 প্রতিস্থাপন করে। সাইবার অপরাধের বিস্তারিত বিধান। |
| **Cyber Security Act** | ২০২৩ | DSA প্রতিস্থাপনকারী নতুন আইন। আরও আধুনিক বিধান। |

---

---

# ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
# অধ্যায় ৮: গণিত
### MCQ: ১৫ নম্বর | লিখিত: ২০ নম্বর
# ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

---

## ৮.১ সংখ্যাতত্ত্ব — বিস্তারিত

### 🔷 LCM ও GCD:
- **GCD (Greatest Common Divisor):** দুটি সংখ্যার সর্বোচ্চ সাধারণ গুণনীয়ক
- **LCM (Least Common Multiple):** দুটি সংখ্যার ক্ষুদ্রতম সাধারণ গুণিতক

**গুরুত্বপূর্ণ সূত্র:**
```
LCM(a, b) × GCD(a, b) = a × b

উদাহরণ: LCM(12, 18) ও GCD(12, 18)
12 = 2² × 3
18 = 2 × 3²
GCD = 2¹ × 3¹ = 6
LCM = 2² × 3² = 36
যাচাই: 36 × 6 = 216 = 12 × 18 ✓
```

### 🔷 মৌলিক সংখ্যা চেনার উপায়:
১ থেকে ১০০ পর্যন্ত মৌলিক সংখ্যা: **2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37, 41, 43, 47, 53, 59, 61, 67, 71, 73, 79, 83, 89, 97** (মোট ২৫টি)

**মনে রাখো:** 1 মৌলিক নয়। 2 একমাত্র জোড় মৌলিক।

### 🔷 ভাজ্যতার নিয়ম:
| কোন সংখ্যা দিয়ে | শর্ত |
|---|---|
| **2 দিয়ে** | শেষ অঙ্ক জোড় (0, 2, 4, 6, 8) |
| **3 দিয়ে** | অঙ্কগুলোর যোগফল 3 দিয়ে বিভাজ্য |
| **4 দিয়ে** | শেষ দুই অঙ্ক 4 দিয়ে বিভাজ্য |
| **5 দিয়ে** | শেষ অঙ্ক 0 বা 5 |
| **6 দিয়ে** | 2 ও 3 উভয়ের নিয়ম মানে |
| **9 দিয়ে** | অঙ্কগুলোর যোগফল 9 দিয়ে বিভাজ্য |
| **11 দিয়ে** | বিজোড় অবস্থানের যোগফল - জোড় অবস্থানের যোগফল = 0 বা 11-এর গুণিতক |

---

## ৮.২ বীজগণিত — বিস্তারিত

### 🔷 সূচক নিয়ম:
```
aᵐ × aⁿ = aᵐ⁺ⁿ         উদাহরণ: 2³ × 2⁴ = 2⁷ = 128
aᵐ ÷ aⁿ = aᵐ⁻ⁿ         উদাহরণ: 2⁵ ÷ 2² = 2³ = 8
(aᵐ)ⁿ = aᵐⁿ            উদাহরণ: (2³)² = 2⁶ = 64
(ab)ᵐ = aᵐbᵐ           উদাহরণ: (2×3)² = 4×9 = 36
a⁰ = 1                  যেকোনো a ≠ 0 এর জন্য
a⁻ⁿ = 1/aⁿ             উদাহরণ: 2⁻³ = 1/8
a^(1/n) = ⁿ√a          উদাহরণ: 8^(1/3) = ∛8 = 2
```

### 🔷 লগারিদম:
```
যদি aˣ = N হয়, তাহলে logₐN = x

মৌলিক নিয়ম:
log(ab) = log a + log b
log(a/b) = log a - log b
log(aⁿ) = n × log a
logₐa = 1
logₐ1 = 0
log₁₀(10) = 1
ln(e) = 1          (e ≈ 2.718)

পরিবর্তন সূত্র: logₐb = log b / log a
```

### 🔷 বর্গ ও ঘন সূত্র:
```
(a + b)² = a² + 2ab + b²
(a - b)² = a² - 2ab + b²
(a + b)(a - b) = a² - b²
(a + b)³ = a³ + 3a²b + 3ab² + b³
(a - b)³ = a³ - 3a²b + 3ab² - b³
a³ + b³ = (a + b)(a² - ab + b²)
a³ - b³ = (a - b)(a² + ab + b²)
```

---

## ৮.৩ ধারা ও অনুক্রম — বিস্তারিত

### 🔷 AP (Arithmetic Progression — সমান্তর ধারা):
যেখানে প্রতিটি পদের পার্থক্য **সমান (d)**।

```
ধারা: a, a+d, a+2d, a+3d, ...

n-তম পদ: aₙ = a + (n-1)d
যোগফল: Sₙ = n/2 × [2a + (n-1)d] = n/2 × (প্রথম পদ + শেষ পদ)
```

**উদাহরণ:** 3, 7, 11, 15, ...  
a = 3, d = 4  
10ম পদ = 3 + (10-1)×4 = 3 + 36 = **39**  
প্রথম ১০ পদের যোগফল = 10/2 × [2×3 + 9×4] = 5 × 42 = **210**

---

### 🔷 GP (Geometric Progression — গুণোত্তর ধারা):
যেখানে প্রতিটি পদের **অনুপাত সমান (r)**।

```
ধারা: a, ar, ar², ar³, ...

n-তম পদ: aₙ = a × r^(n-1)
যোগফল (r ≠ 1): Sₙ = a(rⁿ - 1)/(r - 1)
অসীম GP (|r| < 1): S∞ = a/(1-r)
```

**উদাহরণ:** 2, 6, 18, 54, ...  
a = 2, r = 3  
6ষ্ঠ পদ = 2 × 3⁵ = 2 × 243 = **486**

---

## ৮.৪ শতকরা ও সুদ — বিস্তারিত

### 🔷 শতকরা:
```
x-এর p% = x × p/100

বৃদ্ধি: নতুন মান = পুরনো × (1 + p/100)
হ্রাস:  নতুন মান = পুরনো × (1 - p/100)
```

### 🔷 সরল সুদ (Simple Interest):
```
সুদ (I) = P × R × T / 100
সুদাসল (A) = P + I = P(1 + RT/100)

যেখানে P = আসল, R = বার্ষিক হার (%), T = সময় (বছর)
```

**উদাহরণ:** ৫০,০০০ টাকা ৮% হারে ৩ বছরে সরল সুদ?
```
I = 50000 × 8 × 3 / 100 = ১২,০০০ টাকা
সুদাসল = ৫০,০০০ + ১২,০০০ = ৬২,০০০ টাকা
```

### 🔷 চক্রবৃদ্ধি সুদ (Compound Interest):
```
সুদাসল (A) = P × (1 + R/100)ᵀ
সুদ = A - P
```

**উদাহরণ:** ৫০,০০০ টাকা ১০% চক্রবৃদ্ধি হারে ২ বছরে?
```
A = 50000 × (1 + 10/100)² = 50000 × 1.21 = ৬০,৫০০ টাকা
সুদ = ৬০,৫০০ - ৫০,০০০ = ১০,৫০০ টাকা
```

---

## ৮.৫ Binary গণিত — বিস্তারিত

### 🔷 Binary যোগ:
```
নিয়ম:
0 + 0 = 0
0 + 1 = 1
1 + 0 = 1
1 + 1 = 10  (carry 1)
1 + 1 + 1 = 11  (carry 1)
```

**উদাহরণ:**
```
  1 0 1 1 0 1    (45)
+ 0 1 1 0 1 1    (27)
-----------
 1 0 0 1 0 0 0   (72)
```

### 🔷 1's Complement ও 2's Complement:
Binary subtraction ও negative সংখ্যার জন্য:

```
1's Complement: সব বিট উল্টে দাও
1011 → 0100

2's Complement: 1's Complement + 1
0100 + 1 = 0101
```

**2's Complement দিয়ে বিয়োগ (A - B = A + 2's Complement of B):**
```
1010 - 0011 = ?
2's Complement of 0011 → 1's = 1100 → +1 = 1101
1010 + 1101 = 10111 → Carry বাদ দিলে → 0111 = 7 ✓
```

---

---

# ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
# অধ্যায় ৯: সাধারণ জ্ঞান (IT বিষয়ক)
### MCQ: ১০ নম্বর
# ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

---

## ৯.১ বাংলাদেশে IT ইতিহাস — বিস্তারিত

| ঘটনা | বিস্তারিত তথ্য |
|---|---|
| **প্রথম কম্পিউটার** | IBM-1620, বাংলাদেশ পরমাণু শক্তি কমিশন, **১৯৬৪** সাল (আইয়ুব খানের আমলে) |
| **প্রথম ডিজিটাল টেলিফোন** | ১৯৯০ সালে |
| **ইন্টারনেট শুরু** | ১৯৯৬ সালে (সীমিত আকারে), ব্যাপকভাবে ১৯৯৯ সালে |
| **প্রথম সাইবার ক্যাফে** | বনানী, ঢাকা, **১৯৯৯** সাল |
| **প্রথম মোবাইল কোম্পানি** | **CityCell** (Pacific Telecom), **১৯৯৩** সাল |
| **সাবমেরিন ক্যাবল** | **২১ মে ২০০৬**, SEA-ME-WE-4, কক্সবাজার (Cox's Bazar) এ সংযুক্ত |
| **3G চালু** | **১৪ অক্টোবর ২০১২**, টেলিটক |
| **4G চালু** | **১৯ ফেব্রুয়ারি ২০১৮** |
| **প্রথম দেশীয় ল্যাপটপ** | **দোয়েল** — টেশিস (TESHIS) কর্তৃক তৈরি |
| **প্রথম সার্চ ইঞ্জিন** | **পিপীলিকা** (Pipilika), **১৩ এপ্রিল ২০১৩** (SUST) |
| **প্রথম ডিজিটাল জেলা** | **যশোর** |
| **প্রথম WiFi নগর** | **সিলেট** |
| **প্রথম হাইটেক পার্ক** | কালিয়াকৈর হাইটেক পার্ক (গাজীপুর) |
| **ডিজিটাল বাংলাদেশ ঘোষণা** | **২০০৮** সালে (আওয়ামী লীগের নির্বাচনী ইশতেহার) |
| **Bangladesh Computer Council (BCC)** | প্রতিষ্ঠিত ১৯৮৩ সালে |
| **দ্বিতীয় সাবমেরিন ক্যাবল** | SEA-ME-WE-5, **২০১৭** সালে |

---

## ৯.২ গুরুত্বপূর্ণ IT ব্যক্তিত্ব — বিস্তারিত

| নাম | পরিচয় | গুরুত্বপূর্ণ অবদান |
|---|---|---|
| **Charles Babbage** | কম্পিউটারের জনক (ব্রিটিশ, ১৭৯১-১৮৭১) | Analytical Engine ও Difference Engine উদ্ভাবন |
| **Ada Lovelace** | প্রথম প্রোগ্রামার (ব্রিটিশ) | Analytical Engine-এর জন্য প্রথম Algorithm লেখেন |
| **Alan Turing** | কম্পিউটার বিজ্ঞানের জনক (ব্রিটিশ) | Turing Machine, AI ধারণা, WWII কোড ভাঙা |
| **John von Neumann** | আধুনিক কম্পিউটার আর্কিটেকচারের প্রবক্তা | Von Neumann Architecture (CPU + Memory + I/O) |
| **Bill Gates** | Microsoft প্রতিষ্ঠাতা | Windows OS, BASIC |
| **Steve Jobs** | Apple প্রতিষ্ঠাতা | Macintosh, iPod, iPhone, iPad |
| **Linus Torvalds** | Linux উদ্ভাবক (ফিনিশ) | Linux Kernel (১৯৯১), Git |
| **Tim Berners-Lee** | World Wide Web উদ্ভাবক (ব্রিটিশ) | HTTP, HTML, URL (১৯৮৯-৯১) |
| **Vint Cerf & Bob Kahn** | Internet-এর জনক | TCP/IP Protocol উদ্ভাবন |
| **Dennis Ritchie** | C ভাষার উদ্ভাবক | C Language, UNIX (Ken Thompson-এর সাথে) |
| **James Gosling** | Java-এর উদ্ভাবক | Java Programming Language |
| **Guido van Rossum** | Python-এর উদ্ভাবক | Python Language (১৯৯১) |
| **Mark Zuckerberg** | Facebook প্রতিষ্ঠাতা | Social Media |
| **Larry Page & Sergey Brin** | Google প্রতিষ্ঠাতা | Google Search Engine (১৯৯৮) |

---

## ৯.৩ গুরুত্বপূর্ণ পূর্ণরূপ — সম্পূর্ণ তালিকা

| সংক্ষিপ্ত | পূর্ণরূপ |
|---|---|
| **CPU** | Central Processing Unit |
| **RAM** | Random Access Memory |
| **ROM** | Read Only Memory |
| **ALU** | Arithmetic Logic Unit |
| **CU** | Control Unit |
| **PC** | Program Counter (বা Personal Computer) |
| **MAR** | Memory Address Register |
| **MDR** | Memory Data Register |
| **URL** | Uniform Resource Locator |
| **HTML** | HyperText Markup Language |
| **HTTP** | HyperText Transfer Protocol |
| **API** | Application Programming Interface |
| **GUI** | Graphical User Interface |
| **CLI** | Command Line Interface |
| **IoT** | Internet of Things |
| **AI** | Artificial Intelligence |
| **ML** | Machine Learning |
| **DL** | Deep Learning |
| **VPN** | Virtual Private Network |
| **ISP** | Internet Service Provider |
| **GPS** | Global Positioning System |
| **USB** | Universal Serial Bus |
| **BIOS** | Basic Input/Output System |
| **UEFI** | Unified Extensible Firmware Interface |
| **VLSI** | Very Large Scale Integration |
| **OCR** | Optical Character Recognition |
| **OMR** | Optical Mark Recognition |
| **ASCII** | American Standard Code for Information Interchange |
| **Unicode** | Universal Character Encoding Standard |
| **DBMS** | Database Management System |
| **RDBMS** | Relational Database Management System |
| **SQL** | Structured Query Language |
| **LAN** | Local Area Network |
| **WAN** | Wide Area Network |
| **MAN** | Metropolitan Area Network |
| **IP** | Internet Protocol |
| **TCP** | Transmission Control Protocol |
| **UDP** | User Datagram Protocol |
| **DNS** | Domain Name System |
| **DHCP** | Dynamic Host Configuration Protocol |
| **FTP** | File Transfer Protocol |
| **SSH** | Secure Shell |
| **SSL** | Secure Sockets Layer |
| **TLS** | Transport Layer Security |
| **VoIP** | Voice over Internet Protocol |
| **NIC** | Network Interface Card |
| **MAC** | Media Access Control |
| **OSI** | Open Systems Interconnection |
| **RISC** | Reduced Instruction Set Computer |
| **CISC** | Complex Instruction Set Computer |
| **OOP** | Object-Oriented Programming |
| **SDLC** | Software Development Life Cycle |
| **IDE** | Integrated Development Environment |
| **OS** | Operating System |
| **FIFO** | First In First Out |
| **LIFO** | Last In First Out |
| **DDoS** | Distributed Denial of Service |
| **MFA/2FA** | Multi-Factor Authentication / Two-Factor Authentication |
| **IaaS** | Infrastructure as a Service |
| **PaaS** | Platform as a Service |
| **SaaS** | Software as a Service |
| **SSD** | Solid State Drive |
| **HDD** | Hard Disk Drive |
| **DRAM** | Dynamic Random Access Memory |
| **SRAM** | Static Random Access Memory |
| **AES** | Advanced Encryption Standard |
| **RSA** | Rivest–Shamir–Adleman (তিন উদ্ভাবকের নামে) |
| **MD5** | Message Digest 5 |
| **SHA** | Secure Hash Algorithm |
| **ATM** | Automated Teller Machine |
| **EFT** | Electronic Funds Transfer |
| **QR** | Quick Response (QR Code) |
| **NFC** | Near Field Communication |
| **RFID** | Radio Frequency Identification |
| **ERP** | Enterprise Resource Planning |
| **CRM** | Customer Relationship Management |
| **IDE** | Integrated Development Environment |
| **API** | Application Programming Interface |
| **JSON** | JavaScript Object Notation |
| **XML** | Extensible Markup Language |
| **CSS** | Cascading Style Sheets |
| **AJAX** | Asynchronous JavaScript and XML |

---

## ৯.৪ বাংলাদেশের IT সংস্থা — সম্পূর্ণ

| সংক্ষিপ্ত | পূর্ণরূপ | কাজ |
|---|---|---|
| **BTRC** | Bangladesh Telecommunication Regulatory Commission | টেলিযোগাযোগ নিয়ন্ত্রণ |
| **BTCL** | Bangladesh Telecommunications Company Limited | সরকারি টেলিফোন সেবা |
| **BCC** | Bangladesh Computer Council | কম্পিউটার প্রসার ও উন্নয়ন |
| **ICT Division** | Information and Communication Technology Division | IT নীতিমালা ও উন্নয়ন |
| **a2i** | Aspire to Innovate | ডিজিটাল সরকারি সেবা |
| **BASIS** | Bangladesh Association of Software and Information Services | সফটওয়্যার শিল্প সংগঠন |
| **ISPAB** | Internet Service Providers Association of Bangladesh | ISP সংগঠন |
| **PGCB** | Power Grid Company of Bangladesh | বিদ্যুৎ সঞ্চালন |
| **DESCO** | Dhaka Electric Supply Company | ঢাকার বিদ্যুৎ বিতরণ |
| **DPDC** | Dhaka Power Distribution Company | ঢাকার বিদ্যুৎ বিতরণ |
| **PDB** | Bangladesh Power Development Board | বিদ্যুৎ উৎপাদন |
| **BREB** | Bangladesh Rural Electrification Board | গ্রামীণ বিদ্যুৎ |

---

---

# ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
# বিগত পরীক্ষার প্রশ্ন ও পূর্ণাঙ্গ উত্তর
### বাংলাদেশ ব্যাংক AME (CS) লিখিত পরীক্ষা ২০১৯
# ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

---

### ✅ প্রশ্ন ১: Distributed DBMS কী? এর বৈশিষ্ট্যসমূহ বর্ণনা করো।

**সংজ্ঞা:** DDBMS হলো এমন একটি ডেটাবেজ ম্যানেজমেন্ট সিস্টেম যেখানে ডেটাবেজ একটি কম্পিউটারে কেন্দ্রীভূত না থেকে নেটওয়ার্কে সংযুক্ত একাধিক কম্পিউটারে বিতরণ করা থাকে, কিন্তু ব্যবহারকারীর কাছে এটি একটি একীভূত সিস্টেম হিসেবে দেখায়।

**উদাহরণ:** বাংলাদেশ ব্যাংকের ATM নেটওয়ার্ক — ঢাকা, চট্টগ্রাম, সিলেটে আলাদা ডেটাবেজ সার্ভার থাকলেও গ্রাহক যেকোনো ATM থেকে তার account-এ সমান অ্যাক্সেস পান।

**বৈশিষ্ট্য:**
1. **Location Transparency:** ডেটা কোথায় সংরক্ষিত তা ব্যবহারকারীকে জানতে হয় না
2. **Replication Transparency:** একই ডেটা একাধিক স্থানে থাকলেও ব্যবহারকারী একটি কপিই দেখেন
3. **Hardware Independence:** বিভিন্ন ধরনের হার্ডওয়ারে কাজ করতে পারে
4. **OS Independence:** বিভিন্ন অপারেটিং সিস্টেমে চলতে পারে
5. **Network Independence:** বিভিন্ন নেটওয়ার্ক প্রোটোকলে কাজ করে
6. **DBMS Independence:** বিভিন্ন ডেটাবেজ সফটওয়্যারের সাথে কাজ করতে পারে
7. **Distributed Transaction Management:** একাধিক সাইটে লেনদেন সামঞ্জস্যপূর্ণভাবে পরিচালনা করা

---

### ✅ প্রশ্ন ২: Distributed Banking System-এ ATM কীভাবে Test করা যায়?

**ATM Testing Strategy:**

**Functional Testing:**
- কার্ড সন্নিবেশ ও PIN যাচাই
- Balance inquiry সঠিক কিনা
- নির্দিষ্ট পরিমাণ উত্তোলন
- Transaction receipt প্রিন্টিং

**Network Testing:**
- ব্যাংকের Central Server-এর সাথে সংযোগ যাচাই
- নেটওয়ার্ক বিচ্ছিন্নতায় ATM-এর আচরণ
- Timeout handling

**Security Testing:**
- PIN Encryption যাচাই
- Card skimming রোধ
- Session timeout

**Database Testing (DDBMS-এ):**
- Real-time balance update (টাকা কাটা হলে সাথে সাথে balance কমছে কিনা)
- Concurrent transaction — দুটো ATM থেকে একই account-এ একসাথে টাকা তুললে কী হয়
- ACID properties মেনে চলছে কিনা

**Load Testing:**
- Peak hour-এ (ঈদের সময়) অনেক transaction একসাথে
- Server response time

---

### ✅ প্রশ্ন ৩: Web Application Development-এ Application Framework-এর গুরুত্ব কী?

[বিস্তারিত উত্তর অধ্যায় ৪.৪-এ দেওয়া আছে]

**সংক্ষেপে:** Framework = কাঠামো যা কোড পুনর্ব্যবহার, নিরাপত্তা, MVC আর্কিটেকচার ও দ্রুত উন্নয়ন নিশ্চিত করে।

---

### ✅ প্রশ্ন ৪: Micro ও Macro (Monolithic) Kernel-এর পার্থক্য কী? Windows NT-এর I/O Manager?

[বিস্তারিত উত্তর অধ্যায় ৫.২-এ দেওয়া আছে]

---

### ✅ প্রশ্ন ৫: Node, Hub, Backbone, Router ও Gateway

[বিস্তারিত উত্তর অধ্যায় ২.৩-এ দেওয়া আছে]

---

---

# ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
# পরীক্ষার কৌশল ও বিশেষ টিপস
# ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

---

## 🎯 MCQ পরীক্ষার জন্য — বিস্তারিত কৌশল

### দ্রুত মনে রাখার পদ্ধতি:
1. **OSI স্তর:** "All People Seem To Need Data Processing" (7 থেকে 1)
2. **Port Numbers:** 20/21=FTP, 22=SSH, 23=Telnet, 25=SMTP, 53=DNS, 80=HTTP, 110=POP3, 143=IMAP, 443=HTTPS
3. **Sorting Best:** Merge Sort — সবসময় O(n log n)
4. **Bluetooth Piconet:** সর্বোচ্চ **৭টি** Slave
5. **RISC = ARM = Smartphone**
6. **Universal Gate = NAND ও NOR**

### MCQ-এ সাধারণ যে প্রশ্নগুলো আসে:
- OSI Model-এর কোন স্তরে কোন ডিভাইস/প্রোটোকল
- TCP vs UDP পার্থক্য
- Cache প্রকারভেদ ও কাজ
- RISC vs CISC
- Sorting Complexity
- SQL কমান্ডের ধরন (DDL/DML/DCL)
- ACID Properties
- Number System রূপান্তর
- Logic Gate (Universal Gate)
- Encryption প্রকারভেদ

---

## 📝 লিখিত পরীক্ষার কৌশল:

### উত্তর লেখার কাঠামো:
```
১. সংজ্ঞা (২-৩ বাক্য)
২. বৈশিষ্ট্য/বিবরণ (বুলেট পয়েন্ট)
৩. তুলনা সারণি (যদি পার্থক্য জিজ্ঞেস করে)
৪. উদাহরণ (বাস্তব, বাংলাদেশ প্রেক্ষাপটে)
৫. Diagram/চিত্র (সম্ভব হলে)
```

### নম্বর বাড়ানোর কৌশল:
- টেবিল ও চিত্র আঁকো — পরীক্ষক খুশি হয়
- বাংলাদেশ ব্যাংকের ATM, DBMS উদাহরণ দাও — প্রাসঙ্গিক মনে হয়
- হেডিং-সাবহেডিং সুন্দরভাবে লেখো
- পরিচ্ছন্ন হাতের লেখা

---

## 📅 ৬ সপ্তাহের পড়ার পরিকল্পনা

| সপ্তাহ | বিষয় | প্রতিদিন |
|---|---|---|
| **১ম সপ্তাহ** | কম্পিউটার নেটওয়ার্কিং (সম্পূর্ণ) | OSI, TCP/IP, Protocol, Device, IP |
| **২য় সপ্তাহ** | DBMS + SQL (সম্পূর্ণ) | ER Diagram, Normalization, SQL, ACID |
| **৩য় সপ্তাহ** | Computer Architecture + OOP | CPU, Memory, Gates + Encapsulation, Inheritance |
| **৪র্থ সপ্তাহ** | OS + Data Structure | Process, Scheduling, Deadlock + Stack, Queue, Tree |
| **৫ম সপ্তাহ** | Cyber Security + সাধারণ জ্ঞান | Encryption, Attack, Cloud + IT ইতিহাস |
| **৬ষ্ঠ সপ্তাহ** | গণিত + মডেল টেস্ট | Number, Algebra, Binary + পূর্ণ Revision |

---

## ⚡ শেষ মুহূর্তের জন্য সবচেয়ে গুরুত্বপূর্ণ তথ্য

```
OSI 7 স্তর:     Application, Presentation, Session, Transport, Network, Data Link, Physical
TCP/IP 4 স্তর:  Application, Transport, Internet, Network Access
গুরুত্বপূর্ণ Port: HTTP=80, HTTPS=443, FTP=21, SSH=22, DNS=53, SMTP=25
Sorting:        Merge Sort = সবসময় O(n log n)
Stack = LIFO, Queue = FIFO
ACID:           Atomicity, Consistency, Isolation, Durability
OOP নীতি:      Encapsulation, Inheritance, Polymorphism, Abstraction
Deadlock শর্ত: Mutual Exclusion, Hold & Wait, No Preemption, Circular Wait
Universal Gate: NAND ও NOR
RISC:           ARM, স্মার্টফোনে ব্যবহার, কম বিদ্যুৎ
Cache:          L1 (দ্রুততম, CPU-এ), L2, L3
RAM:            DRAM (Main Memory), SRAM (Cache)
Bluetooth:      সর্বোচ্চ 7টি Slave
বাংলাদেশ কম্পিউটার: IBM-1620, ১৯৬৪
সাবমেরিন ক্যাবল: ২১ মে ২০০৬, কক্সবাজার
```

---

> 🎯 **শিক্ষকের চূড়ান্ত পরামর্শ:**
> 
> ১. **বোঝো, মুখস্থ নয়** — বুঝলে পরীক্ষার হলে যেকোনো প্রশ্নেই উত্তর করতে পারবে।
> ২. **বিগত প্রশ্ন বারবার পড়ো** — একই বিষয় বারবার আসে।
> ৩. **লিখে লিখে পড়ো** — হাতে লিখলে মনে থাকে বেশি।
> ৪. **প্রতিদিন একটু একটু** — শেষ রাতে পড়ার চেয়ে নিয়মিত ভালো।
> ৫. **বাংলাদেশ প্রেক্ষাপট** — উদাহরণে বাংলাদেশ ব্যাংক, DESCO, ATM নেটওয়ার্ক ব্যবহার করো।
>
> **শুভকামনা রইলো! তুমি পারবে! 🎯🚀**

---

*গাইডটি বাংলাদেশ ব্যাংক ও বিভিন্ন মন্ত্রণালয়ের পূর্ববর্তী প্রশ্নপত্র বিশ্লেষণের ভিত্তিতে তৈরি।*
*সর্বশেষ আপডেট: ২০২৫*
