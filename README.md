# How-to-handle-the-LauncherClick-event-in-WPF-Ribbon-control-

This repository contains a sample that shows how to handle the `LauncherClick` event in the Syncfusion WPF Ribbon control. In this sample, a `RibbonWindow` hosts a `Ribbon` with multiple tabs, and the `LauncherClick` event is wired to the **New** `RibbonBar` in the HOME tab.

The launcher button is displayed at the lower-right corner of a `RibbonBar`. By handling the `LauncherClick` event, you can execute custom logic when the launcher button is clicked, such as opening a dialog or showing related commands. The event handler is declared in the code-behind and connected directly from XAML.

```XAML
<syncfusion:RibbonBar Name="Clipboard" Header="Clipboard" LauncherClick="Clipboard_LauncherClick"/>
```
```C#
//The code to handle the above event 
void ribbonbar_LauncherClick(object sender, RoutedEventArgs e)
{
    //events actions
}
```
This approach is useful when a RibbonBar needs extra actions beyond the visible controls in the ribbon while keeping the UI compact and organized.

Output:

![WPF_Ribbon_LauncherButton](Ribbon_LauncherButton.png)