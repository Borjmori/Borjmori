import pandas as pd
import yfinance as yf

# تعریف نماد سهم برای دریافت داده‌های تاریخی
symbol = "AAPL"

# تاریخ شروع و پایان جمع آوری داده‌های تاریخی
start_date = "2010-01-01"
end_date = "2022-04-23"

# دریافت داده‌های تاریخی با استفاده از کتابخانه yfinance
stock_data = yf.download(symbol, start=start_date, end=end_date)

# نمایش ۵ ردیف اول داده‌های تاریخی
print(stock_data.head())
