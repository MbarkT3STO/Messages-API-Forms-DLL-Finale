# About
# -----------------------------------------------------------------
A simple DLL to show Error, Success and Confirm messages for WinForms (.NET) projects

# 1st Step (Add reference)
# -----------------------------------------------------------------
- **1 -** Open your WinForms project using visual studio.
- **2 -** Go to Solution Explorer
- **3 -** Right click on References
- **4 -** Chose Add Reference
- **5 -** Click on Browse
- **6 -** Select all downloaded DLLs
- **7 -** Click on OK

# 2nd Step (Using)
# -----------------------------------------------------------------
- First thing you sould do is inside your **.cs** Form code use the **Name Space** :  

```
using Messages_API_Forms_DLL;
```

- At this time this DLLs covering just thre type of messages, are : **Error**, **Success** and **Confirm**.

Now if you want to show a message just create a new object from a specific class [**ERROR** , **SUCCESS** , **CONFIRM**], and send it a message to show after that show the new object.

# Examples
# -----------------------------------------------------------------
- **Show Error Message**
```
ERROR E = new ERROR("Text to show");
E.ShowDialog();
```

- **Show Success Message**
```
SUCCESS S = new SUCCESS("Text to show");
S.ShowDialog();
```

- **Show Confirm Message**
```
CONFIRM C = new CONFIRM("Text to show");
C.ShowDialog();
```

# Important Notes :
# -----------------------------------------------------------------
- **1 -** If you have a form created he can inherit the properties and design from DLLs (He can inherit just from one Class [**ERROR** or **SUCCESS** or **CONFIRM**])
- **2 -** The **Confirm** form contains three buttons: [**Yes** , **No** , **Cancel**]
- The click on **Yes** Button will return a **DialogResult.Yes**, and close the form.
- The click on **No** Button will return a **DialogResult.No**, and close the form.


# This Library is totaly free
