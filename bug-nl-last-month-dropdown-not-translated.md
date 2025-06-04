# Bug: Dropdown values under "Last Month" are not translated into selected language (NL)

**Status:** Open  
**Severity:** Medium  
**Priority:** Medium  
**Environment:**  
- Website: [https://***.com]
- License: SCB (e.g., Brazil)  
- Language: Dutch (NL)  
- Browser: Safari 
- OS: Sequoia 15.3

---

## 🐾 Steps to Reproduce:

1. Navigate to [https://***.com]
2. In the top-right corner, select SCB license (e.g., Brazil)
3. Change language to Dutch (NL)  
   _(also reproducible with other non-English, non-German, non-Arabic, non-Chinese locales)_
4. Hover over menu section **[Markten]** (Markets)
5. Click on menu item **[Alle markten]** (All Markets)
6. Scroll to the block **"Wij bieden naadloos handelen"** ("We offer seamless trading")
7. Click any link to an instrument (e.g., **[Gold]**)
8. Navigate to the tab **[Historische gegevens]** (Historical data)
9. Open the dropdown **[Last Month]**

---

## ✅ Expected Result:

The dropdown values under **[Last Month]** are translated into the selected language (e.g., Dutch)

---

## ❌ Actual Result:

The dropdown values are displayed in **English** regardless of the selected language

---

## 🔁 Reproducibility:

100% — Issue occurs consistently under the specified conditions.
