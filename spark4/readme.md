Apache Spark 4 introduces a powerful new capability, among many others: **Python Data Source API**. This means we can now create our own `spark.read.format(...)` implementations entirely in Python, extending Spark’s native data reading capabilities without needing Java or Scala. 

Imagine reading complex or niche file formats — like **PDFs** — directly into Spark DataFrames, enabling richer, scalable analytics workflows that weren’t possible before.

The notebook in this directory contains an implementation of `spark.read.format('pdf')` data source. It uses **pdfplumber** as the underlying PDF parsing tool.
