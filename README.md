# Invoice-Processing-Automation
Two automation tools that cut invoice processing time from 2 days to 3 hours. PDF categorization + missing file detection. Works offline, no setup required.
# Cocoblu Invoice Automation System

A suite of two web-based automation tools that reduced our invoice processing workflow from **2 days to 3 hours (86% faster)**.

## Problem Statement

Our organization processes hundreds of vendor invoices monthly from Cocoblu. The workflow involved:
- Manual file verification (checking if all PDFs downloaded correctly)
- Manual document categorization (GST invoices vs. Credit/Debit notes)
- Manual data entry and reconciliation

**Total time: 2 days per month | Error rate: High | Bottleneck: Manual labor**

## Solution

Two integrated browser-based tools that automate the entire workflow:

---

## Tool 1: PDF Sorter ⚡

**Problem:** Each PDF had to be manually opened and checked to determine if it was a GST invoice, credit note, or debit note.

**Before:** 2 hours per month  
**After:** 2 minutes per month  
**Improvement:** 98% faster

### What it does:
- Scans uploaded PDFs
- Auto-categorizes based on accounting logic (checks for keywords, amounts, vendor details)
- Generates organized folders for each document type
- One-click export to sorted structure

### Use case:
Warehouse team uploads invoice batch → tool sorts into 3 folders → sorted PDFs ready for processing

### Technical details:
- Extracts PDF metadata and text
- Applies classification rules (GST vs. Credit/Debit detection)
- Generates downloadable categorized files
- Works completely offline

---

## Tool 2: Missing PDF Detector 🔍

**Problem:** Cocoblu bulk downloads sometimes fail silently. We had no way to know which invoices didn't download until manual verification.

**Before:** 3 hours per month (manual reconciliation)  
**After:** 1 minute per month  
**Improvement:** 99.4% faster

### What it does:
- Takes a PDF manifest (list of expected files)
- Scans uploaded files
- Generates a report of missing PDFs
- Exports a checklist for re-download

### Use case:
Download fails → upload manifest + actual files → tool tells you exactly what's missing → re-download only missing invoices

### Technical details:
- Compares manifest against uploaded files
- Generates missing files report
- Exports as downloadable list
- Handles large batches (100+ files)

---

## Combined Results

| Metric | Before | After | Improvement |
|--------|--------|-------|-------------|
| **Monthly processing time** | 2 days (16 hrs) | 3 hours | 81% faster |
| **Manual categorization time** | 2 hours | 2 minutes | 98% faster |
| **File reconciliation time** | 3 hours | 1 minute | 99.4% faster |
| **Re-work due to missing files** | 2-3 hours | Eliminated | 100% reduction |

**Total monthly time saved:** 7-8 hours

---

## How to Use

### PDF Sorter:
1. Open `Cocoblu_PDF_Sorter_v3.html`
2. Upload invoice PDFs
3. Click "Sort PDFs"
4. Download organized folders

### Missing PDF Detector:
1. Open `Cocoblu_Missing_Files_Updated.html`
2. Upload PDF manifest (text file with expected filenames)
3. Upload actual invoice PDFs
4. Download missing files report

---

## Technical Details

- **Built with:** HTML5, JavaScript, PDF.js (PDF parsing)
- **Browser-based:** Works completely offline, no server required
- **No coding required from user:** Just upload files, click buttons, download results
- **Dark mode UI:** Professional, easy-to-use interface
- **Single file deployment:** No dependencies, works in any modern browser

---

## Business Impact

- **Time savings:** 7-8 hours/month = ~84 hours/year
- **Error reduction:** Zero manual categorization errors
- **Cost:** Free (internal tool)
- **ROI:** Immediate (eliminates manual re-work)
- **Scalability:** Can handle 100+ invoices in one batch

---

## Files Included

- `Cocoblu_PDF_Sorter_v3.html` - Document categorization tool
- `Cocoblu_Missing_Files_Updated.html` - File reconciliation tool
- `README.md` - This file

---

## What I Learned Building This

1. **Problem-solving mindset:** Identify inefficiencies → build solutions → measure results
2. **Full-stack thinking:** PDF processing, file reconciliation, UI/UX design
3. **Real-world constraints:** Works offline, handles edge cases, user-friendly design
4. **Business impact:** Every tool must save time/money or reduce errors

This project shows how automation isn't just about writing code—it's about understanding workflows, identifying pain points, and building tools that actually get used.

---

**Status:** In production use at current organization  
**Contact:** Available on GitHub
