# E-Commerce ETL Pipeline

## Overview
Built SSIS pipeline to extract, transform, and load 541K+ records

## Pipeline Flow
OLE DB Source → Data Conversion → Calculated Columns → Conditional Split → SQL Server

## What Was Done
✓ Extracted 541K+ records from source
✓ Converted data types (string to numeric, datetime)
✓ Calculated derived column: LineTotal (Quantity × UnitPrice)
✓ Handled NULL and negative values
✓ Applied conditional validation
✓ Loaded to SQL Server destination

## Key Components
- Source: OLE DB (online_retail table)
- Transformation: Data validation and conversion
- Destination: SQL Server database
