# Grade-Book-App
# 🎓 Student Grades Utility

A simple yet powerful JavaScript project to calculate and analyze student grades. This utility provides functions to compute class averages, evaluate grades, check passing statuses, and generate personalized performance messages.

---

## ✨ Features

- **📊 Calculate Average Score:** Effortlessly compute the average of a list of scores.
- **📝 Grade Evaluation:** Determine grades based on score thresholds.
- **✅ Pass/Fail Check:** Instantly verify if a score meets the passing criteria.
- **📢 Performance Message:** Generate a detailed summary including class average, individual grades, and pass/fail status.

---

## 🛠️ Code Overview

```javascript
function getAverage(scores) {
    let sum = 0;

    for (const score of scores) {
      sum += score;
    }

    return sum / scores.length;
}

function getGrade(score) {
    if (score === 100) {
      return "A++";
    } else if (score >= 90) {
      return "A";
    } else if (score >= 80) {
      return "B";
    } else if (score >= 70) {
      return "C";
    } else if (score >= 60) {
      return "D";
    } else {
      return "F";
    }
}

function hasPassingGrade(score) {
    return getGrade(score) !== "F";
}

function studentMsg(totalScores, studentScore) {
    let passFail;
    if (hasPassingGrade(studentScore)) {
        passFail = "You passed the course.";
    } else {
        passFail = "You failed the course.";
    }
    return "Class average: " + getAverage(totalScores) + ". Your grade: " + getGrade(studentScore) + ". " + passFail;
}

console.log(studentMsg([92, 88, 12, 77, 57, 100, 67, 38, 97, 89], 37));
```

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

