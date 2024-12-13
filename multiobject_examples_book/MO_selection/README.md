
### Key Points to Understand:

**Multi-target selection is not the same as multi-target optimization!**

- **Multi-target optimization** considers multiple properties simultaneously in both prediction and utility space. It can be implemented using **MultiBgolearn** in Python.
  
- **Multi-target selection** typically considers two properties independently and then combines them in either the property space or utility space using a Pareto front. A method is constructed to select one solution from the points on the Pareto front. This can be implemented using **BgoKit** in Python.

---

**Note:** We are not claiming that one approach is better than the other; they are fundamentally different. Multi-target optimization truly accounts for the interdependencies between properties, whereas multi-target selection treats properties more independently.

---

If you are still unclear about the differences, please refer to the video for further explanation.

