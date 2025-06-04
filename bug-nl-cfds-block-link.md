# Bug: Entire block "De voordelen van CFD's op aandelen" is incorrectly displayed as a hyperlink

**Status:** Open  
**Severity:** Low  
**Priority:** Medium  
**Environment:**  
- Website: [https://***.com] 
- License: SCB (CYSEC) — e.g., Estonia  
- Language: Dutch (NL)  
- Browser: Safari 
- OS: Sequoia 15.2

---

## 🐾 Steps to Reproduce:

1. Navigate to [https://***.com]
2. In the top-right corner, select license SCB (CYSEC) — e.g., Estonia
3. Switch website language to Dutch (NL)
4. Hover over the menu section **[Markten]** (Markets)
5. Click on menu item **[Aandelen]** (Shares)
6. Scroll to the content block titled **"De voordelen van CFD's op aandelen"** ("The benefits of CFDs on shares")

---

## ✅ Expected Result:
The block **"De voordelen van CFD's op aandelen"** is displayed as regular static text.

---

## ❌ Actual Result:
The entire block **"De voordelen van CFD's op aandelen"** is rendered as a clickable hyperlink, which is not expected.

---

## 📝 Notes:
- This issue seems to be locale-specific (Dutch language with SCB license).
- In the EN version or under other licenses, this block behaves correctly.
