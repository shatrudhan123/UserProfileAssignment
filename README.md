# Android User Profile Assignment

This project is an Android application developed as part of an assignment to display a user profile by fetching data from an API and presenting it in a clean and responsive UI.

---

## 📱 Features

- Fetch and display user profile data
- Show user details:
  - Name
  - Username
  - Avatar image
  - Location (City, Country)
  - Followers & Following count
  - Website and social media links
- Clickable website and Instagram profile
- Loading indicator while fetching data
- Clean and responsive UI
- MVVM architecture

---

## 🛠 Tech Stack

- **Language:** Kotlin  
- **UI:** XML  
- **Architecture:** MVVM  
- **Networking:** Retrofit  
- **Image Loading:** Glide  
- **Async Handling:** Coroutines + LiveData  

---

## ⚠️ API Note (Important)

The API URL provided in the assignment was:

https://raw.githubusercontent.com/android-assessment/profile/refs/heads/main/data.json


While implementing the assignment, this API was returning **404 (Not Found)** and the referenced GitHub repository was not accessible.  
This issue was verified using both **browser** and **Postman**.

### ✅ Solution
To avoid blocking the assignment, a **public mock API** was created using **GitHub Gist**, maintaining the same response structure as required.  
This mock API was then integrated into the application using Retrofit.

This approach ensures:
- All assignment requirements are fulfilled
- Real-world handling of unavailable backend services
- Clean and maintainable code

---

## 📡 Mock API Response Structure

```json
{
  "name": "Bruno Pham",
  "username": "brunopham",
  "avatar": "https://i.pravatar.cc/300",
  "location": {
    "city": "Da Nang",
    "country": "Vietnam"
  },
  "followers": 220,
  "following": 150
}

