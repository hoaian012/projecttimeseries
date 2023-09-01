# projecttimeseries
## Hướng dẫn các hàm trong dự án:
- sl_lagar: lựa chọn độ trễ để chạy mô hình ar

- sl_lagma: lựa chọn độ trễ để chạy mô hình ma

- modelar(df_train, df_test): Hàm truyền tham số dữ liệu train, test, chạy mô hình ar và trả về giá trị rmsle & predict return

- modelma(df_train, df_test): Hàm truyền tham số dữ liệu train, test, chạy mô hình ma và trả về giá trị rmsle & predict return

- modelarima(df_train, df_test): Hàm truyền tham số dữ liệu train, test, chạy mô hình arima và trả về giá trị rmsle & predict return

- modelautoarima(df_train, df_test): Hàm truyền tham số dữ liệu train, test, chạy mô hình auto_arima và trả về giá trị rmsle & predict return

- select_cp(result): lựa chọn cổ phiếu dựa trên kết quả mô hình đã chọn

## Các bước tiến hành chạy mô hình theo dự án:
- B1: Thu thập dữ liệu, có thể thôn qua việc download data trên các website chứng khoán
  
- B2: Xử lý dữ liệu, đưa các dữ liệu về đúng kiểu float, set ngày là index theo ngày (theo tần suất ngày làm việc)

- B3: Chạy mô hình modelar, modelma, arima, auto arima để ra các kết quả mô hình

- B4: Chạy hàm select_cp để lựa chọn các cổ phiếu theo tiêu chí đề ra từ các kết quả mô hình
