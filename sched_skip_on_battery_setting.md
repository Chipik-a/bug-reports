# Test Case: Scheduler Skip When on Battery and Cosmos Setting Enabled

**Status:** To Verify  
**Type:** Feature Validation / Conditional Scheduler Behavior  
**Component:** fsscan Scheduler  
**Environment:**  
- Device: Laptop (with battery power status)  
- Product Version: 25.2.408
- Logs: ***.log  

---

## 🧪 Test Objective

Verify that when the new **Cosmos boolean setting** is set to **true**, and **---** is started with the option `--sched` while the laptop is running on battery, the scan **does not start** and the status returned is `"skipped"`.

---

## ⚙️ Precondition / Setup

- boolean setting: **true** (set via portal configuration)
- Laptop is running on battery (not plugged in)

---

## 🐾 Steps to Reproduce:

1. Set the *** setting `skip_scan_on_battery` to **true** on the portal.
2. Ensure the laptop is running on battery power (unplug power cable).
3. Run the command: C:\Program Files (x86)\***.exe –sched  
4. Monitor the scan behavior and check the logs (`***.log`).

---

## ✅ Expected Result:

- **** **does not start scanning**.
- Status reported:  "*****"
- Log entry indicating the skip reason due to battery power and cosmos setting enabled.

---

## ❌ Actual Result:

*(To be filled during testing)*

---

## 📝 Notes:

- The *** setting should be adjustable on the portal by the user or admin.
- Scan behavior should dynamically respect power source changes (if scanning scheduled while plugged, unplugging should affect next scan).
- Verify no scan processes start when on battery with setting enabled.

---

## 📎 Attachments (Optional):

- Log excerpts showing `"skipped"` status
- Screenshot of portal settings for the cosmos boolean flag

