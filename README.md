# [HomePage](http://bgolearn.caobin.asia/) 
This repository provides code demonstrations and data to illustrate the application of Bgolearn in materials design. [BiliBili](https://m.bilibili.com/video/BV1LTtLeaEZp?buvid=Y345CE3557236F9745C19B291052E1114B47&is_story_h5=false&mid=cKE7LXHZdUdBetZbd%2FNVln8FTQ%2FSZMtL1rElX6M3iMo%3D&plat_id=240&share_from=ugc&share_medium=iphone&share_plat=ios&share_source=WEIXIN&share_tag=s_i&timestamp=1726650391&unique_k=fyJEJqG&up_id=3546615870654962)



---

### Key Points to Understand:

**Multi-target selection is not the same as multi-target optimization!**

- **Multi-target optimization** considers multiple properties simultaneously in both prediction and utility space. It can be implemented using **MultiBgolearn** in Python.
  
- **Multi-target selection** typically considers two properties independently and then combines them in either the property space or utility space using a Pareto front. A method is constructed to select one solution from the points on the Pareto front. This can be implemented using **BgoKit** in Python.


**Note:** We are not claiming that one approach is better than the other; they are fundamentally different. Multi-target optimization truly accounts for the interdependencies between properties, whereas multi-target selection treats properties more independently.


If you are still unclear about the differences, please refer to the [video](https://m.bilibili.com/video/BV1LTtLeaEZp?buvid=Y345CE3557236F9745C19B291052E1114B47&is_story_h5=false&mid=cKE7LXHZdUdBetZbd%2FNVln8FTQ%2FSZMtL1rElX6M3iMo%3D&plat_id=240&share_from=ugc&share_medium=iphone&share_plat=ios&share_source=WEIXIN&share_tag=s_i&timestamp=1726650391&unique_k=fyJEJqG&up_id=3546615870654962) for further explanation.

