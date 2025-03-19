# PulseAPI Documentation for C# (WinForms / WPF)

Welcome to the **PulseAPI** for C# developers! This API offers various functions that you can use in your WinForms or WPF applications. The use of the API is free of charge, but you must include a **notice stating that the PulseAPI from PulseExternal is being used** in your application.

---

## Usage Requirement

Ensure you include the following `using` directive at the beginning of your C# file:

```csharp
// Import API
using PulseAPI;
```

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

## **PulseAPI.Api** – The Main Class

This class provides general functions for linking to external pages.

### a) **YouTube()**

Opens your YouTube channel in the default browser.

**Usage:**

```csharp
private void YTbtn_Click(object sender, RoutedEventArgs e)
{
  PulseAPI.Api.YouTube();
}
```

### b) **Discord()**

Opens your Discord server in the default browser.

**Usage:**

```csharp
private void DCbtn_Click(object sender, RoutedEventArgs e)
{
PulseAPI.Api.Discord();
}
```

### c) **Github()**

Opens your GitHub profile in the default browser.

**Usage:**

```csharp
private void GHbtn_Click(object sender, RoutedEventArgs e)
{
PulseAPI.Api.Github();
}
```

---

## **PulseAPI.RobloxAPI** – Roblox-Specific Functions

This class contains functions for interacting with the Roblox application and retrieving user information.

### a) **KillRoblox()**

Terminates the Roblox application if it is open.

**Usage:**

```csharp
PulseAPI.RobloxAPI.KillRoblox();
```

### b) **OpenRoblox()**

Starts the Roblox application.

**Usage:**

```csharp
PulseAPI.RobloxAPI.OpenRoblox();
```

### c) **RestartRoblox()**

Restarts Roblox by closing and reopening the application.

**Usage:**

```csharp
PulseAPI.RobloxAPI.RestartRoblox();
```

### d) **GetUsername()**

Retrieves the username of the currently logged-in Roblox account.

**Usage:**

```csharp
string username = PulseAPI.RobloxAPI.GetUsername();
```

### e) **GetDisplayname()**

Retrieves the display name of the current Roblox user.

**Usage:**

```csharp
string displayName = PulseAPI.RobloxAPI.GetDisplayname();
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
string description = PulseAPI.RobloxAPI.GetDescription();
```

### h) **GetTotalFriends()**

Returns the number of friends of the current Roblox user.

**Usage:**

```csharp
int totalFriends = PulseAPI.RobloxAPI.GetTotalFriends();
```

### i) **GetTotalGroups()**

Returns the number of groups the current Roblox user is a member of.

**Usage:**

```csharp
int totalGroups = PulseAPI.RobloxAPI.GetTotalGroups();
```

### j) **GetCreatedDate()**

Returns the creation date of the current Roblox account.

**Usage:**

```csharp
DateTime createdDate = PulseAPI.RobloxAPI.GetCreatedDate();
```

### k) **GetBannedStatus()**

Checks if the current Roblox user is banned.

**Usage:**

```csharp
bool isBanned = PulseAPI.RobloxAPI.GetBannedStatus();
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

This documentation describes the use of the **PulseAPI** in C# for WinForms and WPF applications. If you have any questions or issues, contact PulseExternal.

