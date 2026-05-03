# Python Learning Tracker — Data Analyst (7 ngày)

> **Bắt đầu:** 18/04/2026
> **Mục tiêu:** Đủ sức làm bài test Python cho vị trí Data Analyst
> **Thời gian:** 3–4 giờ/ngày

---

## Tổng quan tiến độ

| Ngày | Chủ đề                               | Trạng thái | Điểm tự đánh giá |
| ----- | --------------------------------------- | ------------ | ---------------------- |
| Day 1 | Python Basics nâng cao                 | [ ]          | — / 10                |
| Day 2 | NumPy                                   | [ ]          | — / 10                |
| Day 3 | Pandas cơ bản                         | [ ]          | — / 10                |
| Day 4 | Pandas nâng cao                        | [ ]          | — / 10                |
| Day 5 | Visualization & EDA                     | [ ]          | — / 10                |
| Day 6 | SQL trong Python & Bài toán thực tế | [ ]          | — / 10                |
| Day 7 | Mock Test & Ôn tổng                   | [ ]          | — / 10                |

**Trạng thái:** `[ ]` Chưa làm &nbsp;|&nbsp; `[~]` Đang làm &nbsp;|&nbsp; `[x]` Hoàn thành

---

## Day 1 — Python Basics nâng cao

**Folder:** [`day1_python_basics/`](../day1_python_basics/)
**Ngày làm:** 18/04/2026
**Thời gian thực tế:** ___ giờ

### Checklist lý thuyết

- [X] List comprehension
- [X] Dict comprehension
- [X] Lambda, `map()`, `filter()`, `zip()`
- [X] `*args`, `**kwargs`

### Checklist bài tập

- [ ] Lọc số chẵn và bình phương bằng list comprehension
- [ ] Tạo dict từ 2 list dùng `zip()`
- [ ] Viết hàm tính moving average
- [ ] Bài tập thêm từ Exercism / LeetCode

### Ghi chú & điểm cần nhớ

```
(Ghi lại các syntax dễ quên, trick hay, lỗi đã gặp)
```

---

## Day 2 — NumPy

**Folder:** [`day2_numpy/`](../day2_numpy/)
**Ngày làm:** ___/___/2026
**Thời gian thực tế:** ___ giờ

### Checklist lý thuyết

- [ ] `ndarray`, shape, dtype
- [ ] Indexing, slicing, boolean masking
- [ ] `np.mean`, `np.std`, `np.percentile`, `np.where`
- [ ] Broadcasting

### Checklist bài tập

- [ ] Tạo 100 điểm ngẫu nhiên, tính mean/std/median
- [ ] Lọc outlier ngoài 2 std
- [ ] Normalize dữ liệu về [0, 1]
- [ ] Bài tập thêm

### Ghi chú & điểm cần nhớ

```

```

---

## Day 3 — Pandas cơ bản ⭐

**Folder:** [`day3_pandas_basics/`](../day3_pandas_basics/)
**Ngày làm:** ___/___/2026
**Thời gian thực tế:** ___ giờ
**Dataset dùng:** ___________________

### Checklist lý thuyết

- [ ] `DataFrame`, `Series`, đọc CSV
- [ ] `head()`, `info()`, `describe()`
- [ ] `loc` vs `iloc`
- [ ] Boolean filtering
- [ ] Xử lý missing: `isnull()`, `fillna()`, `dropna()`

### Checklist bài tập

- [ ] Load dataset, kiểm tra shape và dtype
- [ ] Tìm các dòng theo điều kiện lọc
- [ ] Xử lý toàn bộ missing values
- [ ] Thêm cột tính toán mới
- [ ] Bài tập thêm

### Ghi chú & điểm cần nhớ

```

```

---

## Day 4 — Pandas nâng cao ⭐

**Folder:** [`day4_pandas_advanced/`](../day4_pandas_advanced/)
**Ngày làm:** ___/___/2026
**Thời gian thực tế:** ___ giờ

### Checklist lý thuyết

- [ ] `groupby()` + aggregation
- [ ] `agg()` với nhiều hàm
- [ ] `merge()` — 4 loại join
- [ ] `pivot_table()`
- [ ] `apply()` với custom function

### Checklist bài tập

- [ ] Tính KPI (mean/sum/count) theo nhiều nhóm
- [ ] `agg` nhiều hàm cùng lúc
- [ ] Join 2 bảng, kiểm tra kết quả
- [ ] Tạo pivot table doanh thu
- [ ] Bài tập thêm

### Ghi chú & điểm cần nhớ

```

```

---

## Day 5 — Visualization & EDA

**Folder:** [`day5_visualization_eda/`](../day5_visualization_eda/)
**Ngày làm:** ___/___/2026
**Thời gian thực tế:** ___ giờ

### Checklist lý thuyết

- [ ] `matplotlib` cơ bản — figure, axes, labels
- [ ] `seaborn` — histplot, boxplot, barplot, heatmap

### Checklist bài tập

- [ ] Vẽ distribution của cột numeric
- [ ] Correlation heatmap
- [ ] Top 10 theo doanh thu (barplot nằm ngang)
- [ ] Boxplot phát hiện outlier
- [ ] Hoàn thành 1 EDA report từ đầu đến cuối

### Ghi chú & điểm cần nhớ

```

```

---

## Day 6 — SQL trong Python & Bài toán thực tế ⭐

**Folder:** [`day6_sql_realworld/`](../day6_sql_realworld/)
**Ngày làm:** ___/___/2026
**Thời gian thực tế:** ___ giờ

### Checklist lý thuyết

- [ ] Pandas replicate SQL (WHERE, GROUP BY, ORDER BY, HAVING)
- [ ] Xử lý datetime: `pd.to_datetime`, `dt.month`, `dt.year`
- [ ] `value_counts()`, `nunique()`, `duplicated()`

### Checklist bài tập

- [ ] Cohort analysis — tỷ lệ giữ chân khách hàng
- [ ] RFM segmentation
- [ ] Rolling 7-day average doanh thu
- [ ] Top / Bottom 10% customers
- [ ] Bài tập thêm từ StrataScratch

### Ghi chú & điểm cần nhớ

```

```

---

## Day 7 — Mock Test & Ôn tổng

**Folder:** [`day7_mocktest/`](../day7_mocktest/)
**Ngày làm:** ___/___/2026
**Thời gian thực tế:** ___ giờ

### Mock Test Checklist

- [ ] Data Cleaning (duplicate, missing, wrong dtype)
- [ ] Aggregation — tính KPI theo nhóm
- [ ] Merge nhiều bảng
- [ ] Visualization — vẽ chart thể hiện insight
- [ ] Viết nhận xét / insight từ data

### Điểm yếu cần ôn thêm

```
(Ghi lại sau khi mock test)
```

### Tự đánh giá tổng thể

- Sẵn sàng cho bài test: [ ] Chưa &nbsp;|&nbsp; [ ] Tạm ổn &nbsp;|&nbsp; [ ] Sẵn sàng

---

## Checklist kỹ năng tổng hợp

> Tick khi tự giải được trong < 10 phút không cần tra cứu.

- [ ] `groupby` + `agg` nhiều hàm cùng lúc
- [ ] `merge` đúng loại join (left/right/inner/outer)
- [ ] Xử lý datetime (to_datetime, dt.month, dt.year, dt.days)
- [ ] `value_counts()`, `nunique()`, `duplicated()`
- [ ] Sort + lấy top N
- [ ] `apply` với lambda trên từng dòng/cột
- [ ] Boolean indexing nhiều điều kiện
- [ ] Normalize / scale dữ liệu
- [ ] Phát hiện và xử lý outlier
- [ ] Vẽ được 4 loại chart cơ bản

---

## Tài nguyên

| Nguồn        | Link                                | Dùng cho                     |
| ------------- | ----------------------------------- | ----------------------------- |
| Kaggle Learn  | https://www.kaggle.com/learn/pandas | Bài học Pandas có notebook |
| StrataScratch | https://www.stratascratch.com       | Bài test DA thực tế        |
| Exercism      | https://exercism.org                | Luyện Python cơ bản        |
| LeetCode      | https://leetcode.com                | Bài tập có chấm điểm    |

---

*Cập nhật lần cuối: ___/___/2026*
