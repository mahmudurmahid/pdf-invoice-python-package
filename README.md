# 📄 PDF Invoice Generator – Python Package

A lightweight Python package designed to automate the conversion of Excel-based invoices into professionally formatted PDF documents. Ideal for businesses seeking to streamline their invoicing processes.

---

## 📖 Table of Contents

- [🚀 Features](#-features)
- [🛠 Installation](#-installation)
- [📦 Usage](#-usage)
- [🧪 Testing](#-testing)
- [🧰 Tools & Technologies](#-tools--technologies)
- [📚 Learning Resources](#-learning-resources)
- [🙌 Credits](#-credits)
- [📄 License](#-license)

---

## 🚀 Features

- ✅ Batch conversion of Excel invoices to PDF
- 🖼️ Support for custom logo images
- 📁 Auto-creation of output directories
- 📄 Clean formatting and PDF table layouts
- ⚠️ Built-in error handling

---

## 🛠 Installation

```bash
pip install pdf-invoice-generator
```

---

## 📦 Usage

```python
from invoicing import invoice

invoice.generate(
    invoices_path="path/to/excel_invoices",
    pdfs_path="path/to/output_pdfs",
    logo_image_path="path/to/company_logo.png",
    product_id_col="Product ID",
    product_name_col="Product Name",
    amount_purchased_col="Quantity",
    price_per_unit_col="Unit Price",
    total_price_col="Total"
)
```

### Parameters

| Parameter              | Description                              |
| ---------------------- | ---------------------------------------- |
| `invoices_path`        | Directory containing Excel invoice files |
| `pdfs_path`            | Directory to save generated PDF invoices |
| `logo_image_path`      | Path to the company logo image           |
| `product_id_col`       | Column name for product IDs              |
| `product_name_col`     | Column name for product names            |
| `amount_purchased_col` | Column name for quantities purchased     |
| `price_per_unit_col`   | Column name for unit prices              |
| `total_price_col`      | Column name for total prices             |

---

## 🧪 Testing

### ✅ Test Scenarios Checklist

| Feature            | Test Type          | Status    |
| ------------------ | ------------------ | --------- |
| Invoice Conversion | Integration        | ✅ Passed |
| Logo Rendering     | Manual             | ✅ Passed |
| Directory Creation | Unit               | ✅ Passed |
| Column Mapping     | Unit / Integration | ✅ Passed |
| Error Handling     | Unit               | ✅ Passed |

### 🧪 Running Tests

Install testing dependencies:

```bash
pip install pytest
```

Run tests:

```bash
pytest
```

---

## 🧰 Tools & Technologies

```plaintext
Tool/Library     Purpose
---------------  --------------------------------------
Python           Core programming language
pandas           Reading and manipulating Excel data
openpyxl         Working with Excel files
fpdf             Generating PDF documents
pytest           Running unit and integration tests
```

---

## 📚 Learning Resources

```plaintext
- pandas Documentation: https://pandas.pydata.org/docs/
- openpyxl Documentation: https://openpyxl.readthedocs.io/en/stable/
- FPDF Documentation: https://pyfpdf.github.io/fpdf2/
- pytest Documentation: https://docs.pytest.org/en/stable/
```

---

## 🙌 Credits

```plaintext
👨‍💻 Author: Mahmud Urmahid
GitHub: https://github.com/mahmudurmahid
```

---

## 📄 License

```plaintext
MIT License – see the LICENSE file for details.
```
