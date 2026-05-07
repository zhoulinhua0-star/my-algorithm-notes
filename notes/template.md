# Binary Search

## Idea
- Works on sorted array
- Repeatedly divide search space in half
- Compare target with middle element

---

## ⏱ Time & Space Complexity
- Time: O(log n)
- Space: O(1)

---

## ⚠️ Edge Cases
- Empty array
- Target not in array
- Single element

---

## 🔁 Steps
1. Set left = 0, right = n - 1
2. While left <= right:
   - mid = left + (right - left) / 2
   - if arr[mid] == target → return
   - if arr[mid] < target → move left
   - else → move right

---

## 💻 Code (Java)

```java
public class BinarySearch {
    public static int search(int[] arr, int target) {
        int left = 0, right = arr.length - 1;

        while (left <= right) {
            int mid = left + (right - left) / 2;

            if (arr[mid] == target) return mid;
            else if (arr[mid] < target) left = mid + 1;
            else right = mid - 1;
        }
        return -1;
    }
}