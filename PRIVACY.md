## **Context Menu Manager Neo (CMMN) Privacy Policy**

### **1. Overview**

**Context Menu Manager Neo (CMMN)** ("the Application") is a standalone, local Windows desktop utility designed to inspect, manage, back up, and diagnose Windows Explorer context menu registrations.

We take your privacy seriously. **The Application operates 100% offline on your local device. It does not collect, transmit, store on external servers, or share any personal data, personal identifiable information (PII), or telemetry.**

### **2. Data Collection and Network Usage**

- **No Data Collection**: The Application contains no analytics SDKs, no telemetry reporters, no crash uploaders, and no advertising or tracking modules.
- **No Internet Access**: The Application makes zero network connections and does not request the `internetClient` capability in its MSIX package manifest.

### **3. Local Data Processing and Storage**

To provide context menu management and backup/restore functionality, the Application processes and stores data strictly on your local computer.

### **4. System Permissions Disclosure**

The Application declares the following Windows desktop capabilities solely for local functionality:

- **`runFullTrust` & `unvirtualizedResources`**: Required to read and manage real Windows Shell context menu registry keys and to launch the isolated COM sandbox prober (`Prober.exe`).
- **`allowElevation`**: Required so the companion backend process (`Backend.exe`) can request standard Windows UAC elevation when you choose to modify system-wide (`HKEY_LOCAL_MACHINE`) context menu entries.

### **5. Third-Party Sharing**

Because the Application collects no information and has no network functionality, no data is ever sold, transferred, or shared with the developer or any third party.

### **6. Data Retention and Deletion**

All data created by the Application resides on your local device under your full control. You can remove all local settings and backups at any time by:

- Uninstalling the Application via **Windows Settings -> Apps -> Installed apps**; and/or
- Deleting the `%LocalAppData%\CMMN` directory (or the application folder in Portable Mode) and the `HKEY_CURRENT_USER\Software\CMMN` registry key.

### **7. Changes and Contact Us**

If we update this Privacy Policy, we will post the revised version on this page and update the Effective Date above.
If you have any questions about this Privacy Policy, please contact us via the project's repository Issues page or the publisher support email listed on the Microsoft Store page.
