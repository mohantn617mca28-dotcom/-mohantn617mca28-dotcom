<h1 align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=35&duration=3000&pause=1000&color=00F7FF&center=true&vCenter=true&width=800&lines=Hi+there+%F0%9F%91%8B%2C+I'm+Mohan+K;Full+Stack+Developer+%F0%9F%92%BB;Web+Developer+%F0%9F%8C%90;UI%2FUX+Enthusiast+%F0%9F%8E%A8;Welcome+to+my+GitHub+Profile!" alt="Typing SVG" />
</h1>

<p align="center">
  <img src="https://komarev.com/gh-pvc/?username=MohanK-2026&color=00f7ff&style=for-the-badge&label=PROFILE+VIEWS" alt="Profile Views" />
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">
</p>

## 🌐 About Me

<img align="right" alt="Coding" width="380" src="https://cdn.dribbble.com/users/1162077/screenshots/3848914/programmer.gif">

- 🔭 I'm currently working on **Web Development Projects**
- 🌱 I'm currently learning **Advanced Full Stack Technologies**
- 👨‍💻 All of my projects are available at [**mohan-k-nov8.vercel.app**](https://mohan-k-nov8.vercel.app/)
- 💬 Ask me about **React, Next.js, JavaScript, Python**
- 📫 How to reach me: **mohantn617@gmail.com**
- ⚡ Fun fact: **I turn coffee into code ☕➡️💻**

<br clear="both">

---

## 🧩 LeetCode Stats & Activity

<p align="center">
  <a href="https://leetcode.com/u/MohanK_2026/">
    <img src="https://leetcard.jacoblin.cool/MohanK_2026?theme=dark&font=baloo&ext=contest" alt="LeetCode Stats" />
  </a>
</p>

<p align="center">
  <a href="https://leetcode.com/u/MohanK_2026/">
    <img src="https://img.shields.io/badge/LeetCode-Profile_View-FFA116?style=for-the-badge&logo=leetcode&logoColor=black" alt="LeetCode Profile" />
  </a>
</p>

---

## 💡 Featured LeetCode Solutions

<p align="center">
  <img src="https://img.shields.io/badge/C-%2300599C.svg?style=flat-square&logo=c&logoColor=white" />
  <img src="https://img.shields.io/badge/C++-%2300599C.svg?style=flat-square&logo=c%2B%2B&logoColor=white" />
  <img src="https://img.shields.io/badge/Java-%23ED8B00.svg?style=flat-square&logo=openjdk&logoColor=white" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
</p>

<!-- ================= PROBLEM 1 ================= -->
<details>
<summary><b>🟢 0001. Two Sum (Easy)</b></summary>

<br>

<details>
<summary><b>🔵 C Solution</b></summary>

```c
#include <stdlib.h>

int* twoSum(int* nums, int numsSize, int target, int* returnSize) {
    *returnSize = 2;
    int* result = (int*)malloc(2 * sizeof(int));
    for (int i = 0; i < numsSize; i++) {
        for (int j = i + 1; j < numsSize; j++) {
            if (nums[i] + nums[j] == target) {
                result[0] = i;
                result[1] = j;
                return result;
            }
        }
    }
    *returnSize = 0;
    return NULL;
}
