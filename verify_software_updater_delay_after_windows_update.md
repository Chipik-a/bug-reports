# Test Verification: Delay Software Updater After Windows Update

**Status:** Verified ✅  
**Type:** Logic Validation / Post-Update Behavior  
**Component:** Software Updater Scheduler  
**Environment:**  
- OS: Windows 11  
- Product Version: [25.2.343]  
- Logs: ***.log

---

## 🧪 Test Objective

Ensure the product **does not trigger software updates immediately after a Windows update**, unless **4 hours** have passed since the last software update.

---

## 🔄 Behavior Scenarios

### ✅ Expected Behavior:

1. **Case 1** – Windows Update ➝ Product Update  
 → No action needed, everything is in order.

2. **Case 2** – Product Update ➝ Windows Update  
 → Product should **wait at least 4 hours** from the last software update before re-triggering an update check.

---

## 🐾 Steps to Verify:

1. **Install the product**.
2. Simulate or allow a **software update** (record timestamp).
3. Perform a **Windows Update** after the software update.
4. Monitor behavior of the **Software Updater** component via logs.
5. Ensure it does **not start update check** until 4+ hours have passed since the last product update.

---

## 📋 Logs to Check:

- `***.log` (look for scheduling/rescheduling behavior)
- `***.log` or Windows Event Viewer (to confirm timing of OS updates)
- Registry (optional): check stored timestamp of last update if available

---

## 🔁 Additional Checks:

- Repeat with various update sequences (OS ➝ software and software ➝ OS).
- Test under conditions with:
  - Multiple sequential Windows updates.
  - System time changed manually.

---

## 🗂 Notes:

- This logic prevents excessive updater load after system patches.
- Helps avoid redundant update triggers after patch cycles.

---

## 📎 Attachments (Optional):

- [ ] Screenshot of task logs
- [ ] Excerpt from `updater.log` showing 4h delay
- [ ] Event Viewer timestamps

