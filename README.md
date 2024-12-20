# Grade-Book-App
# 🎓 Student Grades Utility

A simple yet powerful JavaScript project to calculate and analyze student grades. This utility provides functions to compute class averages, evaluate grades, check passing statuses, and generate personalized performance messages.

---

![image](https://github.com/user-attachments/assets/c376b208-f12b-4d0a-8cee-41533ce344de)


## ✨ Features

- **📊 Calculate Average Score:** Effortlessly compute the average of a list of scores.
- **📝 Grade Evaluation:** Determine grades based on score thresholds.
- **✅ Pass/Fail Check:** Instantly verify if a score meets the passing criteria.
- **📢 Performance Message:** Generate a detailed summary including class average, individual grades, and pass/fail status.

---


---

## 🖥️ Example Output

Running the script with the provided example:

```bash
Class average: 71.7. Your grade: F. You failed the course.
```

---

## 🚀 Installation

1. Clone the repository or copy the script into your project.
2. Ensure you have Node.js installed to execute the script.

---

## 📚 Usage

1. Import or include the functions in your project.
2. Call `studentMsg(totalScores, studentScore)` with:
   - An array of scores (`totalScores`).
   - An individual student score (`studentScore`).

### Example

```javascript
const scores = [92, 88, 12, 77, 57, 100, 67, 38, 97, 89];
const studentScore = 85;

console.log(studentMsg(scores, studentScore));
```

**Output:**

```bash
Class average: 71.7. Your grade: B. You passed the course.
```

---

## 🤝 Contributing

Contributions are always welcome! Feel free to:
- Submit a pull request.
- Open an issue.
- Share your feedback.

---

## 📜 License

This project is licensed under the MIT License. See the LICENSE file for details.

---

### 🌟 Happy Coding!

