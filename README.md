# Android API Integration App

## 📱 Overview

This Android application demonstrates **API integration**, **user authentication**, and **dynamic data display** using Retrofit. It connects to the [VU-NIT3213 API](https://nit3213api.onrender.com/) to authenticate users, fetch dashboard data, and display item details.

---

## 🚀 Features

- 🔐 **Login screen**: Authenticate with username and password.
- 📊 **Dashboard screen**: Dynamically displays a list of entities based on the user's keypass.
- 🧾 **Detail screen**: Shows more information for a selected entity.
- 🔄 Retrofit-based networking
- 🧪 Unit test-ready architecture
- 🪛 Modular and scalable design

---

## 🧰 Tech Stack

- Kotlin
- Retrofit2
- AndroidX
- RecyclerView
- Serializable model passing
- Optional: Hilt (for DI), JUnit (for tests)

---

## 🌐 API Details

- **Base URL**: `https://nit3213api.onrender.com/`

### 🔑 Endpoints

| Endpoint | Method | Description |
|---------|--------|-------------|
| `/login` | POST | Returns `keypass` for valid user credentials |
| `/dashboard/{keypass}` | GET | Returns list of dynamic `Entity` objects |
| `/dashboard/{keypass}/{entityId}` | GET | (Optional) Retrieves a specific entity |

---

## 🛠️ Setup Instructions

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   ```

2. **Open in Android Studio**

3. **Build & Run** on emulator or real device (API 23+)

4. **Login using credentials** (example):
   ```
   Username: John
   Password: s12345678
   ```

---

## 📂 Project Structure

```
├── MainActivity.kt            # Login screen
├── DashboardActivity.kt       # Dashboard list screen
├── DetailsActivity.kt         # Entity detail screen
├── adapter/EntityAdapter.kt   # RecyclerView adapter
├── LoginRequest.kt
├── LoginResponse.kt
├── DashboardResponse.kt
├── Entity.kt
├── di/
│   ├── ApiService.kt
│   └── RetrofitClient.kt
├── res/layout/
│   ├── activity_main.xml
│   ├── activity_dashboard.xml
│   ├── activity_details.xml
│   └── item_entity.xml
```

---

## 🧪 Example Test

```kotlin
class LoginRequestTest {
    @Test
    fun testLoginRequest() {
        val login = LoginRequest("John", "s12345678")
        assertEquals("John", login.username)
        assertEquals("s12345678", login.password)
    }
}
```

---

## ✍️ Author

- **Name**: Mohit Roka Chhetri(s8113967)
- **Course**: NIT3213 Mobile Application Development
- **Year**: 2025

---

## 📝 License

This project is for academic purposes under [VU NIT3213](https://www.vu.edu.au/) curriculum. Do not distribute without permission.
