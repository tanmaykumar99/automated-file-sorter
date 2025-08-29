# Automatic File Sorter in File Explorer

A Python script that automatically sorts **CSV (`.csv`)**, **Excel (`.xlsx`)**, and **SQL (`.sql`)** files in a specified folder into dedicated subfolders, and does so periodically
every day.

This helps keep your files organized without manual effort.

---

## Features

- Sorts `.csv` files into a `csv files` folder.
- Sorts `.xlsx` files into a `xlsx files` folder.
- Sorts `.sql` files into a `sql files` folder.
- Automatically creates folders if they don’t exist.
- Logs all file movements to the console.
- Safe: skips files that are not CSV, XLSX, or SQL.

---

## Requirements

- Python 3.6 or higher
- No external packages required

Install dependencies with:
```
pip install -r requirements.txt
```
