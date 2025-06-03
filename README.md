# 🏨 Hostel Room Allocation Automation using RPA (UiPath)

## 📌 Project Overview

This project automates the process of allocating hostel rooms to students based on their **gender**, **preferences**, and **room availability**, using **UiPath Robotic Process Automation (RPA)**. The traditional manual allocation method is often time-consuming, error-prone, and lacks transparency. Our RPA solution replicates the logic of a human administrator and enhances it by introducing repeatability, fairness, and efficiency.

## 🎯 Objectives

- ✅ Fair and transparent room allocation
- ✅ Two-phase allocation strategy (preference-first, fallback-second)
- ✅ Automated email notifications to students
- ✅ Excel-based structured data input and output
- ✅ Scalable and modular RPA design

## 🛠️ Technologies Used

- **UiPath Studio** (Main automation logic)
- **Excel** (Student and room data input/output)
- **SMTP/Email Integration** (Notifications)


## 📋 Input Format

### 🧑 Student Data (`sample.xlsx` - Sheet1)
| Student ID | Name      | Email               | Gender | Room Preference |
|------------|-----------|---------------------|--------|------------------|
| 101        | Alice     | alice@example.com   | F      | Single           |
| 102        | Bob       | bob@example.com     | M      | Double           |

### 🏠 Room Data (`sample.xlsx` - Sheet2)
| Room Number | Gender | Capacity | Occupied |
|-------------|--------|----------|----------|
| 101         | F      | 1        | 0        |
| 102         | M      | 2        | 1        |

## ⚙️ How It Works

1. **Read Input Data** from Excel (`sample.xlsx`).
2. **First-Pass Allocation**: Assign students rooms matching their **gender** and **preference**.
3. **Second-Pass Allocation**: Reconsider unallocated students with relaxed room preferences.
4. **Output Results** to Excel sheets:
   - Sheet3: Preference-based allocations
   - Sheet4: Alternate allocations
   - Sheet5: Unallocated students
5. **Send Email Notifications**:
   - Preferred room confirmation
   - Alternate room confirmation
   - Unavailability notice

## ✉️ Email Samples

- ✅ **Preferred Room Allocated**  
- ✅ **Alternate Room Allocated**  
- ❌ **Room Not Allocated**

Each student receives a **personalized email** based on their allocation status.


## 🚀 Future Enhancements

- 🌐 **Web Portal** for real-time status and room change requests
- 🔄 **Live Database Integration** for dynamic updates
- 🤖 **ML-Based Room Satisfaction Prediction**
- 🏢 **Multi-Campus Support** and configuration management

## 👨‍💻 Authors

- [mayur-hegde](https://github.com/mayur-hegde)



