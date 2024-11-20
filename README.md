    distancei = (2 x 3.14 x 180) ÷ (w + h x 360) x 1000 + 3

using the bounding box size (width (`w`) and height (`h`)) detected by an object detection model.

Here’s a simplified explanation of the distance formula in proper Markdown:

---

1. **Bounding Box Size:**
   - **Width (`w`)** and **Height (`h`)** are the dimensions of the bounding box around the object.
   - **Larger bounding box** → Object is closer to the camera.
   - **Smaller bounding box** → Object is farther from the camera.

2. **Formula Explanation:**
   - (w+h×360): Combines the width and height to calculate how "big" the object appears.
   - (2 x 3.14 x 180) ÷ (w + h x 360) : Scales the bounding box size to calculate the distance.
   - ×1000: Converts the distance into meaningful units (e.g., millimeters or centimeters).
   - +3 : Adjusts for small errors caused by the camera or lens setup.

---

## How It Works:

- **Smaller Width (`w`) and Height (`h`):**
  - The denominator (\(w + h \times 360\)) becomes **large**.
  - Result: The calculated distance is **large** (object is far away).

- **Larger Width (`w`) and Height (`h`):**
  - The denominator becomes **small**.
  - Result: The calculated distance is **small** (object is close).

---


- \(2 \times 3.14 \times 180\): A scaling factor to normalize the calculation.
- \(1000\): Converts the output to desired units (e.g., millimeters).
- \(+3\): Ensures the result is always realistic and accounts for small errors in the camera setup.

---

Referance :

https://emaraic.com/blog/distance-measurement
