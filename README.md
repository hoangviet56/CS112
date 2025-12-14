# CS112 - PHÂN TÍCH VÀ THIẾT KẾ THUẬT TOÁN

<div align="center">

![Language](https://img.shields.io/badge/Language-Vietnamese-red)
![Course](https://img.shields.io/badge/Course-CS112-blue)
![Group](https://img.shields.io/badge/Group-12-green)

**Trường Đại học Công nghệ Thông tin - ĐHQG TP.HCM**

</div>

---

## Thành viên Nhóm 12

| Họ và tên | MSSV |
|:---|:---:|
| **Dương Hoàng Việt** | 24520036 |
| **Hồ Hữu Tây** | 24520029 |

---

## Đề bài

Bạn được cung cấp một hoán vị $p$ có độ dài $n$. Bạn có thể thực hiện thao tác sau bất kỳ số lần nào (có thể là 0 lần):

Chọn ba chỉ số phân biệt $i, j, k$ ($1 \le i < j < k \le n$) sao cho thỏa mãn đồng thời hai điều kiện:
1. $p_i = \max(p_j, p_k) + 1$
2. $p_i = \min(p_j, p_k) + 2$

*(Nói cách khác, $p_i$ là số lớn nhất trong bộ ba và lớn hơn hai số kia lần lượt là 1 và 2 đơn vị).*

**Hành động:** Sau khi chọn được bộ 3 hợp lệ, ta cập nhật:
- $p_i := p_i - 2$
- $p_j := p_j + 1$
- $p_k := p_k + 1$

**Yêu cầu:** Hãy xác định hoán vị **nhỏ nhất theo thứ tự từ điển** có thể thu được sau khi thực hiện thao tác trên bất kỳ số lần nào.

### Ví dụ (Example)

**Input:**
```text
5
4
3 2 1 4
5
3 4 5 2 1
5
2 4 5 3 1
7
5 3 4 1 2 6 7
10
2 7 5 1 3 9 4 10 6 8
```

**Output:**
```text
1 3 2 4
1 2 3 5 4
2 4 5 3 1
1 2 3 4 5 6 7
2 3 4 1 5 7 6 8 9 10
```

**Giải thích:**
Ở test case đầu tiên `[3, 2, 1, 4]`, chọn $i=1, j=2, k=3$ (giá trị là $3, 2, 1$). Thỏa mãn điều kiện $3 = \max(2,1)+1$ và $3 = \min(2,1)+2$.
- $p_1$ giảm 2 còn 1.
- $p_2, p_3$ tăng 1 thành 3, 2.
-> Kết quả: `[1, 3, 2, 4]`.

---

## Tiêu chí chấm điểm Report

Các nhóm viết report và nộp với tên file là `<TenNhom>.pdf`.

Để đánh giá một bản báo cáo chất lượng cho bài toán thuật toán này, điểm số sẽ được phân bố dựa trên các tiêu chí sau (Tổng: **10 điểm**):

| Tiêu chí | Điểm | Mô tả chi tiết |
|:---|:---:|:---|
| **1. Phân tích & Ý tưởng thuật toán** | **3.5** | Trình bày rõ ràng luồng tư duy, cách tiếp cận bài toán. Giải thích được tại sao lại chọn giải pháp đó (Greedy, Dynamic Programming, v.v.). |
| **2. Chứng minh tính đúng đắn** | **2.5** | Chứng minh logic toán học hoặc lập luận chặt chẽ để khẳng định thuật toán luôn tìm ra kết quả tối ưu (nhỏ nhất theo từ điển). |
| **3. Đánh giá độ phức tạp** | **2.0** | Phân tích chính xác độ phức tạp thời gian (Time Complexity) và không gian (Space Complexity). Đảm bảo thỏa mãn giới hạn $N \le 2000$. |
| **4. Cài đặt (Implementation)** | **2.0** | Code sạch, đặt tên biến gợi nhớ, có comment giải thích các đoạn quan trọng. Code phải vượt qua các test case ví dụ. |

---

## Công thức tính điểm tổng kết

Điểm cuối cùng của nhóm sẽ được tính theo công thức trọng số như sau:

$$\text{Final Score} = 0.7 \times (\text{Điểm bài tập về nhà}) + 0.3 \times (\text{Điểm báo cáo})$$

* **Điểm bài tập về nhà:** Dựa trên tổng điểm tương ứng của các bài AC trên hệ thông chấm.
* **Điểm báo cáo:** Dựa trên thang điểm 10 ở mục trên.

## Link nộp bài và Slide

Link nộp bài:
- Code: https://codeforces.com/contestInvitation/44059d1dc61aac4e8a15572d98d0ffcdbddf6876
- Report: https://docs.google.com/forms/d/e/1FAIpQLSdAbULvO2Tm82SM8435e-9OgoiThuWN1sTD6EpgP3j3JJ95tQ/viewform?usp=dialog

Link Slide: https://www.canva.com/design/DAG6gmjjDo8/YAxMLtJzH9px9map2KuE_Q/edit?utm_content=DAG6gmjjDo8&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton