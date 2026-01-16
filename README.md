# CS-Fullscreen-Class

*[English](#english) | [Deutsch](#deutsch)*

<a name="english"></a>
## English

### Purpose and Utility
This repository contains a C# class capable of simulating the **F11** key press using the Windows API (`user32.dll`). Its primary use case is to **programmatically toggle fullscreen mode** in Windows Console applications, where F11 is the standard shortcut for this action.

### How it works
The `SetFullscreen` class provides a static method `PressF11()`. When called, it:
1. Constructs an input sequence for pressing down the F11 key.
2. Constructs an input sequence for releasing the F11 key.
3. Sends these inputs to the system using the native `SendInput` function.

This allows developers to force the console into fullscreen mode without requiring user interaction.

### Usage
Include the class in your project and call:
```csharp
CS_Fullscreen_Class.SetFullscreen.PressF11();
```

---

<a name="deutsch"></a>
## Deutsch

### Nutzen und Zweck
Dieses Repository enthält eine C#-Klasse, die das Drücken der **F11**-Taste mithilfe der Windows API (`user32.dll`) simulieren kann. Der Hauptanwendungsfall besteht darin, den **Vollbildmodus in Windows-Konsolenanwendungen programmgesteuert umzuschalten**, da F11 das Standard-Tastenkürzel für diese Aktion ist.

### Funktionsweise
Die Klasse `SetFullscreen` stellt eine statische Methode `PressF11()` bereit. Beim Aufruf passiert Folgendes:
1. Es wird eine Eingabesequenz für das Drücken der F11-Taste erstellt.
2. Es wird eine Eingabesequenz für das Loslassen der F11-Taste erstellt.
3. Diese Eingaben werden über die native `SendInput`-Funktion an das System gesendet.

Dies ermöglicht es Entwicklern, die Konsole ohne Benutzerinteraktion in den Vollbildmodus zu versetzen.

### Verwendung
Binden Sie die Klasse in Ihr Projekt ein und rufen Sie sie auf:
```csharp
CS_Fullscreen_Class.SetFullscreen.PressF11();
```
