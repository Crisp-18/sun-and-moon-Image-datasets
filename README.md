# sun-and-moon-Image-datasets
日月光斑数据集
## 1.数据采集
塔式聚光器实验（王健47号单片定日镜光斑实验）数据采集完成，数据总量如下所示：
![image](https://user-images.githubusercontent.com/92524510/233988738-b613c669-295b-48d6-ae8b-dbfa4ae47a58.png)

2023.4.1当天月相为79%，多云，只有部分时刻能够观测到光斑，效果较差，拍摄结果肉眼几乎看不出来，与之轨迹对应为5月16日。
![image](https://user-images.githubusercontent.com/92524510/233988907-08a29193-2a9c-4628-97ac-45d6d5124095.png)
月光实验效果较好地仅有2023.4.6moon组，月光清晰可见与之轨迹相对应的有2023.3.1sun—2023.3.4sun四组，如下图所示。
![image](https://user-images.githubusercontent.com/92524510/233988969-ef5b1465-20b5-4301-9e6e-7fd15b9bf713.png)
采集光斑示例图和现场拍摄月亮图如下。
![image](https://user-images.githubusercontent.com/92524510/233989007-d226d54e-f94c-401a-b3b5-b12c5d1fd43a.png)
实验现场图：
![image](https://user-images.githubusercontent.com/92524510/233989041-4f5c9041-6ec1-4539-b6a3-d550d2ce70a1.png)

## 2.后续处理

### 2.1数据整理demo
根据阶段的轨迹匹配，将数据进行配对，整理出日月光斑数据集。先整理出小规模数据，方便实验不同模型，评估它们的性能，截取出2023.4.6的21:12-22:12的一小时时段的月光光斑图，和2023.3.2的9:00-10:00的一小时时段的太阳光斑图，两者的轨迹对应关系如下图显示。
![image](https://user-images.githubusercontent.com/92524510/233989181-0557b7ab-5b01-4209-9cb3-6c2ee7221c2f.png)
再截取2023.4.7的凌晨3:00-4:00的一小时时段的月光光斑图，和2023.3.1的14:54-15:54的一小时时段的太阳光斑图，两者的轨迹对应关系如下图显示。
![image](https://user-images.githubusercontent.com/92524510/233989217-bf9c3bfd-ee9d-44b4-86b3-a06ee2587caa.png)
通过匹配，筛选，最后生成日月光斑数据计demo，由sun_demo和moon_demo两个文件夹组成，分别有750张光斑图，共1500张图片，并且按照顺序一一对应。

### 2.2图像处理
使用opencv，进行图像处理，轮廓识别，特征位置提取，截取光斑，日月光斑都可以成功截取。
![1a1189e14cdad37519bc29bbec2aa4b](https://user-images.githubusercontent.com/92524510/233989785-1115a503-f51f-4c64-92dd-37423830571d.png)
![a17b7246d742826561b37182b4fbca8](https://user-images.githubusercontent.com/92524510/233989797-043527ad-3ea2-498f-b6bc-9cc6e0344719.png)
![d5aab0e263223a088a4392da27ca128](https://user-images.githubusercontent.com/92524510/233989809-444b4f06-89e3-4a10-9a3a-aad1fc2c3014.jpg)
![76570b879d9819bcff7a794a8bd6d6e](https://user-images.githubusercontent.com/92524510/233989824-46be1235-722f-43b4-bef2-5bb1491d525f.jpg)
