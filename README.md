# Bank Statement Manager (Google Colab)

An automated tool to parse, store, and analyze bank statements from Ecuadorian banks using **Google Colab**, **SQLite**, and **OCR**.

## Features

- Upload multiple PDF bank statements directly in Colab.
- Automatic parsing of **Banco del Austro** and **Banco del Pacífico** statements.
- OCR support for scanned PDFs with no embedded text.
- Data normalization and cleaning for consistent extraction.
- Storage in **SQLite** database with unique constraints.
- Financial summary tables and interest calculations.
- Payment simulator for calculating months to pay off debt and total interest.

## Installation

Install dependencies using:

```bash
!apt-get update
!apt-get install -y poppler-utils
!apt-get install -y tesseract-ocr
!apt-get install -y tesseract-ocr-spa
!pip install -r requirements.txt
