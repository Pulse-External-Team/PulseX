# PulseAPI Documentation for C# (WinForms / WPF)

👉 **If you have not yet downloaded the PulseAPI, get it [HERE](https://github.com/Pulse-External-Team/PulseX/releases/download/PulseX-OG/PulseAPI.dll).**

Welcome to the **PulseAPI** for C# developers! This API offers various functions that you can use in your WinForms or WPF applications. The use of the API is free of charge, but you must include a **notice stating that the PulseAPI from PulseExternal is being used** in your application.

---

## License Information:

- **Usage**: You are allowed to use the PulseAPI in your WinForms or WPF projects.
- **Credits**: When using the PulseAPI, you must indicate in your application's user interface that you are using the PulseAPI from **PulseExternal**. This notice must be visible to the users.
- **Liability**: You are solely responsible for the use of the PulseAPI in your projects. Any misuse or issues arising from the use of the API are your responsibility. PulseExternal assumes no liability for the use of the API.

### Example of the required notice (WinForms):

```csharp
Label creditsLabel = new Label();
creditsLabel.Text = "This application uses the PulseAPI from PulseExternal.";
creditsLabel.Location = new Point(10, 10); // Label position
this.Controls.Add(creditsLabel);
```

### Example of the required notice (WPF):

```xml
<TextBlock HorizontalAlignment="Left" VerticalAlignment="Top">
    This application uses the PulseAPI from PulseExternal.
</TextBlock>
```

---

# PulseAPI Classes and Functions

### Loading the API

To use the PulseAPI in your C# project, you must include the following `using` directive at the top of your code:

```csharp
using PulseAPI;
```

## **PulseAPI.Api** – The Main Class

This class provides general functions for linking to external pages.

### 1) **YouTube()**

Opens your YouTube channel in the default browser.

**Usage:**

```csharp
private void YTbtn_Click(object sender, EventArgs e)
{
    PulseAPI.Api.YouTube();
}
```

### 2) **Discord()**

Opens your Discord server in the default browser.

**Usage:**

```csharp
private void DCbtn_Click(object sender, EventArgs e)
{
    PulseAPI.Api.Discord();
}
```

### 3) **Github()**

Opens your GitHub profile in the default browser.

**Usage:**

```csharp
private void GHbtn_Click(object sender, EventArgs e)
{
    PulseAPI.Api.Github();
}
```

---

## **PulseAPI.RobloxAPI** – Roblox-Specific Functions

This class contains functions for interacting with the Roblox application and retrieving user information.

### 1) **KillRoblox()**

Terminates the Roblox application if it is open.

**Usage:**

```csharp
private void KillRBXbtn_Click(object sender, EventArgs e)
{
    PulseAPI.RobloxAPI.KillRoblox();
}
```

### 2) **OpenRoblox()**

Starts the Roblox application.

**Usage:**

```csharp
private void OpenRBXbtn_Click(object sender, EventArgs e)
{
    PulseAPI.RobloxAPI.OpenRoblox();
}
```

### c) **RestartRoblox()**

Restarts Roblox by closing and reopening the application.

**Usage:**

```csharp
private void RestartRBXbtn_Click(object sender, EventArgs e)
{
    PulseAPI.RobloxAPI.RestartRoblox();
}
```

### d) **GetUsername()**

Retrieves the username of the currently logged-in Roblox account.

**Usage:**

```csharp
label1.Text = PulseAPI.RobloxAPI.GetUsername();
```

### e) **GetDisplayname()**

Retrieves the display name of the current Roblox user.

**Usage:**

```csharp
label1.Text = PulseAPI.RobloxAPI.GetDisplayname();
```

### f) **GetAvatar()**

Retrieves the avatar image URL of the current Roblox user.

**Usage:**

```csharp
string avatarUrl = PulseAPI.RobloxAPI.GetAvatar();
```

### g) **GetDescription()**

Returns the profile description of the currently logged-in Roblox user.

**Usage:**

```csharp
label1.Text = PulseAPI.RobloxAPI.GetDescription();
```

### h) **GetTotalFriends()**

Returns the number of friends of the current Roblox user.

**Usage:**

```csharp
label1.Text = PulseAPI.RobloxAPI.GetTotalFriends();
```

### i) **GetTotalGroups()**

Returns the number of groups the current Roblox user is a member of.

**Usage:**

```csharp
label1.Text = PulseAPI.RobloxAPI.GetTotalGroups();
```

### j) **GetCreatedDate()**

Get the date where the Roblox Account was created.

**Usage:**

```csharp
label1.Text = PulseAPI.RobloxAPI.GetCreatedDate();
```

### k) **GetBannedStatus()**

Checks if the current Roblox user is banned.

**Usage:**

```csharp
label1.Text = PulseAPI.RobloxAPI.GetBannedStatus();
```

### l) **JoinPlace()**

Allows the user to join a specific Roblox game (Place). The Place ID must be passed as an argument.

**Usage:**

```csharp
PulseAPI.RobloxAPI.JoinPlace("12345678910");
```

---

## Important Usage Notes

1. **Credits:** You must indicate in your application that the PulseAPI from **PulseExternal** is being used.

2. **Disclaimer:** You are solely responsible for using the PulseAPI. PulseExternal assumes no liability for any damages that may arise from its use.

3. **Correct Implementation:** Ensure that you use the API correctly according to this documentation and integrate the required notice visibly in your application.

---

This documentation describes the use of the **PulseAPI** in C# for WinForms and WPF applications. If you have any ques
