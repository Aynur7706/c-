Əla Aynur 😎 indi sənə **Login + Calculator** birlikdə olan layihə üçün tam, səliqəli, professional və birbaşa copy-paste edilə bilən README hazırladım.

Bunu olduğu kimi `README.md` faylına yerləşdirə bilərsən 👇

---

# 🔐🧮 ASP.NET Web Forms Login & Calculator Project

This project is a combined **Login System** and **Calculator Application** built using **ASP.NET Web Forms (C#)**.
It demonstrates session management, ViewState usage, authentication logic, and event-driven programming.

---

## 🚀 Project Features

### 🔐 Login System

* User authentication (username & password validation)
* Session-based failed attempt tracking
* Account lock after 3 failed attempts
* Dynamic CSS feedback (success, error, shake, locked)
* Reset fail counter after successful login

### 🧮 Calculator

* Addition (+)
* Subtraction (-)
* Multiplication (x)
* Division (÷) with zero-check
* Decimal number support
* Plus/Minus toggle (+/-)
* Percentage calculation (%)
* Clear (C) button
* ViewState-based state management

---

# 🔐 Login System – Technical Overview

## Session Management

The system uses Session to store failed login attempts:

```
Session["failCount"]
```

* Initializes fail count on first page load
* Increments counter after wrong login
* Locks account after 3 failed attempts
* Resets counter after successful login

## Default Credentials

```
Username: admin
Password: 1234
```

## Security Logic

* If failed attempts ≥ 3 → Account locked
* If credentials correct → Success message and counter reset
* If credentials wrong → Error message and shake animation

---

# 🧮 Calculator – Technical Overview

## ViewState Usage

Calculator stores data using ViewState:

```
ViewState["firstNumber"]
ViewState["operation"]
ViewState["newEntry"]
```

This allows:

* Storing first number
* Saving selected operator
* Detecting new input
* Preserving data between postbacks

## Operations Logic

The calculator uses switch-case for operations:

* Addition
* Subtraction
* Multiplication
* Division (with zero protection)

Division includes zero-check to prevent runtime errors.

---

# 🛠 Technologies Used

* ASP.NET Web Forms
* C#
* Session State
* ViewState
* Bootstrap
* Event-driven programming

---

# 🎯 Learning Objectives

This project demonstrates:

* Authentication logic
* Session management
* ViewState state handling
* Web Forms lifecycle
* Switch-case logic
* UI feedback handling
* Postback behavior in ASP.NET

---

# 📂 Project Structure

```
/Site.master          → Master Page (Header, Navigation, Footer)
/Home.aspx            → Login Page
/Home.aspx.cs         → Login Logic (Session handling)
/About.aspx           → Calculator Page
/About.aspx.cs        → Calculator Logic (ViewState handling)
```

---

# 🇦🇿 Azərbaycan dilində

Bu layihə **ASP.NET Web Forms və C#** istifadə edilərək hazırlanmış Login və Kalkulyator sistemidir.

## 🔐 Login Hissəsi

* İstifadəçi adı və şifrə yoxlanışı
* Session ilə səhv cəhdlərin sayılması
* 3 səhv cəhddən sonra hesabın bloklanması
* Uğurlu giriş zamanı sayın sıfırlanması

## 🧮 Kalkulyator Hissəsi

* Toplama, çıxma, vurma, bölmə
* 0-a bölməyə qarşı yoxlama
* Faiz və +/- funksiyası
* ViewState vasitəsilə məlumatların saxlanması

Bu layihə Web Forms mühitində state management və event-based programming məntiqini göstərir.

---

# 👩‍💻 Author

Aynur
