---
name: knowledge-note
description: Tạo hoặc cập nhật file .ipynb lưu kiến thức trong các thư mục của repo python. Dùng skill này khi user muốn: tổng hợp kiến thức, ghi lại ghi chú học tập, tạo note cho một chủ đề, hoặc bất cứ khi nào nhắc đến "lưu lại", "tổng hợp kiến thức", "tạo note", "document lại".
---
# Knowledge Note Skill

Skill này tạo và cập nhật file `.ipynb` trong repo python học Data Analyst.

## Cấu trúc repo

```
python/
├── tracking/                   # File tracking tiến độ
├── day1_python_basics/         # List comprehension, lambda, map/filter/zip
├── day2_numpy/                 # ndarray, indexing, broadcasting
├── day3_pandas_basics/         # DataFrame, loc/iloc, missing values
├── day4_pandas_advanced/       # groupby, merge, pivot_table, apply
├── day5_visualization_eda/     # matplotlib, seaborn, EDA
├── day6_sql_realworld/         # SQL trong pandas, datetime, bài toán thực tế
└── day7_mocktest/              # Mock test tổng hợp
```

**Quy tắc đặt tên file:** `snake_case.ipynb`, mô tả ngắn gọn nội dung.

**Quyết định folder:**

| Chủ đề | Folder |
|--------|--------|
| List comprehension, lambda, `*args`/`**kwargs` | `day1_python_basics/` |
| NumPy array, indexing, broadcasting | `day2_numpy/` |
| DataFrame, `loc`, `iloc`, missing values | `day3_pandas_basics/` |
| `groupby`, `merge`, `pivot_table`, `apply` | `day4_pandas_advanced/` |
| matplotlib, seaborn, EDA | `day5_visualization_eda/` |
| SQL trong pandas, datetime, cohort/RFM | `day6_sql_realworld/` |
| Bài test tổng hợp | `day7_mocktest/` |

---

## Cấu trúc file .ipynb

File `.ipynb` gồm xen kẽ **markdown cell** và **code cell**:

```
[markdown] Tiêu đề + mô tả chủ đề
[markdown] ## 1. Định nghĩa / Bản chất
[code]     # ví dụ minh họa đơn giản nhất
[markdown] ## 2. Cú pháp & cách dùng
[code]     # ví dụ cú pháp đầy đủ
[markdown] ## 3. Các trường hợp thực tế
[code]     # bài toán thực tế, dùng dữ liệu mẫu nếu cần
[markdown] ## Lưu ý quan trọng
```

---

## Quy tắc nội dung

**Nguyên tắc quan trọng nhất:** Ngắn gọn nhưng đủ ý — chắt lọc điểm cốt lõi, không copy nguyên văn, không giải thích dài dòng.

**Phạm vi nội dung:**
- Chỉ document **đúng những gì user liệt kê**, không tự ý lấy thêm nội dung khác từ link dù link có nhiều hơn
- Nếu user không liệt kê gì cụ thể, hỏi lại trước khi document

**Cấu trúc — bắt buộc theo dạng:**
```
[markdown] nhóm khái niệm cùng chức năng + mô tả từng cái
[code]     ví dụ riêng cho khái niệm 1
[code]     ví dụ riêng cho khái niệm 2
[code]     ví dụ riêng cho khái niệm 3
```
- Gộp các khái niệm **cùng chức năng** vào 1 markdown (ví dụ: `append/insert/extend` → nhóm "Thêm phần tử")
- Mỗi khái niệm trong nhóm có **1 code cell riêng** ngay sau markdown, theo đúng thứ tự liệt kê

**Markdown cell:**
- Giải thích bằng tiếng Việt, thuật ngữ kỹ thuật giữ tiếng Anh
- Mỗi khái niệm chỉ 1–3 dòng, đủ để hiểu và nhớ
- Dùng `>` blockquote cho điểm dễ nhầm hoặc lưu ý quan trọng
- Không ghi phần Nguồn

**Code cell:**
- Mỗi cell chỉ minh họa đúng 1 khái niệm vừa giải thích ở markdown trên
- Code ngắn gọn — đủ minh họa, không thừa
- Comment ngắn giải thích output nếu không rõ ràng
- Code phải chạy được độc lập (import đầy đủ trong cell đầu)

**Bài tập — bắt buộc thêm sau mỗi nhóm khái niệm:**

Sau các code cell ví dụ của mỗi nhóm, thêm 2 cell:
```
[markdown] ### Luyện tập
           - Đề bài 1: ...
           - Đề bài 2: ...
[code]     # Viết code của bạn ở đây
```
- Đề bài bám sát đúng khái niệm vừa học trong nhóm đó
- Độ khó tăng dần: bài 1 đơn giản, bài 2 thực tế hơn hoặc kết hợp thêm 1 bước
- Đề bài dùng ngữ cảnh thực tế (danh sách học sinh, sản phẩm, điểm số...) thay vì số trừu tượng
- Code cell để trống (chỉ có comment `# Viết code của bạn ở đây`) để user tự làm

---

## Workflow tạo file

### 1. Xác định folder
Dựa vào chủ đề → chọn folder theo bảng trên.

### 2. Đặt tên file
`snake_case.ipynb` — ví dụ: `list_comprehension.ipynb`, `groupby_agg.ipynb`

### 3. Tạo nội dung ipynb
Dùng Write tool với JSON hợp lệ theo format sau:

```json
{
  "nbformat": 4,
  "nbformat_minor": 5,
  "metadata": {
    "kernelspec": {
      "display_name": "Python 3",
      "language": "python",
      "name": "python3"
    },
    "language_info": {
      "name": "python",
      "version": "3.10.0"
    }
  },
  "cells": [
    {
      "cell_type": "markdown",
      "metadata": {},
      "source": ["# Tên Chủ Đề\n", "\n", "Mô tả ngắn — chủ đề này là gì, dùng khi nào."]
    },
    {
      "cell_type": "markdown",
      "metadata": {},
      "source": ["## 1. Định nghĩa / Bản chất\n", "\n", "<giải thích>"]
    },
    {
      "cell_type": "code",
      "execution_count": null,
      "metadata": {},
      "outputs": [],
      "source": ["# ví dụ code"]
    }
  ]
}
```

**Lưu ý JSON:**
- Mỗi dòng trong `source` là 1 string, kết thúc bằng `\n` (trừ dòng cuối)
- Escape đúng: `\"`, `\\n` trong string, `\n` trong source array
- `outputs` luôn là `[]`, `execution_count` luôn là `null`

### 4. Nếu file đã tồn tại
Đọc file hiện tại bằng Read tool, thêm cells mới vào cuối mảng `cells`, không xóa nội dung cũ.