# ML---SoMiHo-team
Here is a presentation of the process of researching, approaching and solving the Child Mind Institute — Problematic Internet Use - a machine learning competition on the Kaggle platform.

https://www.kaggle.com/competitions/child-mind-institute-problematic-internet-use

This document is divided into 3 main parts: Understanding the problem, initial approaches and solutions, finding ways to improve the model.
Each part includes many sub-sections including code and comes with detailed explanations of the motivation, how the models work, why applying that method improves (or at least why we think it will improve the model), etc.

I. Understanding the problem and data set:

II. Initial approaches and solutions
1. Ý tưởng ban đầu:
   Qua tìm hiểu trên internet, chúng tôi thấy có một số thuật toán học máy phổ biến và hiệu quả cho các bài toán trên Kaggle như các thuật Boosting (LGBM, XGBoost, CatBoost) và Bagging (như là Random Forest). Ban đầu do chưa nghiên cứu sâu sắc về bộ dữ liệu, cũng như Random Forest là một thuật toán đã được học trên lớp và rất dễ hiểu, mô hình đầu tiên chúng tôi chỉ dùng Random Forest.
   Mô hình đầu tiên: Dùng pandas để đọc và ghi dữ liệu (tất cả các phiên bản đều như vậy), dùng toàn bộ dữ liệu trong train.csv để học, các giá trị thiếu được xử lý đơn giản, chưa dùng đến file dữ liệu chuỗi thời gian, dùng 1 thuật toán đơn giản là Random Forest.
   Chi tiết:
   ```
   code here
   ```   

III. Improving model
