# vs-csharp-code-snippets
This repository contains set of code snippets that could be reused during the C# code development

## How to add snippet to you Visual Studio
- You can import a snippet to your Visual Studio installation by using the **Code Snippets Manager**. Open it by choosing **Tools** > **Code Snippets Manager**.
- Click the **Import** button.
- Go to the location where you saved the code snippet in the previous procedure, select it, and click **Open**.
- The **Import Code Snippet** dialog opens, asking you to choose where to add the snippet from the choices in the right pane. One of the choices should be **My Code Snippets**. Select it and click **Finish**, then **OK**.
- [More details](https://docs.microsoft.com/en-us/visualstudio/ide/walkthrough-creating-a-code-snippet?view=vs-2019)

## Available Code snippets list
- **ctor_rk** - constructor with formatted xml comment
```csharp
/// <summary>
/// Initializes a new instance of the <see cref="$classname$"/> class
/// </summary>
public $classname$()
{
}
```
- **nrc_rk** - null reference check
```csharp
if ($variable$ == null)
{
    throw new ArgumentNullException(nameof($variable$));
}
```