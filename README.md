
# vs-csharp-code-snippets
This repository contains set of code snippets that could be reused during the C# code development.
You can also find Project Item templates that allows you to create custom Item templates with Visual Studio.

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
- **prt_status** - ASP.NET core API Produces Response Type snippet without response
```csharp
[ProducesResponseType(StatusCodes.$status$)]
```
- **prt_response** - ASP.NET core API Produces Response Type snippet with response
```csharp
[ProducesResponseType(typeof($type$), StatusCodes.$responsestatus$)]
```
- **rgn_rk** - class body skeleton with regions.
```csharp
#region consts                  
#endregion
                  
#region fields                  
#endregion
                  
#region props                  
#endregion
                  
#region ctors
                  
public $classname$()
{
}
#endregion
                  
#region methods
#endregion
                  
#region helpers
#endregion
```

## How to add Item Template to you Visual Studio
Please follow this guide [More Info](https://docs.microsoft.com/en-us/visualstudio/ide/how-to-create-item-templates?view=vs-2019#manually-create-an-item-template) to import item templates from this repository to you local Visual Studio instance

## Available Item Templates

- **EntityService** - created 3 files for your Entity Service (Query, Transaction, Validation)
- **EntityViewModel** - create 2 View Model files that can be used as Create or update Entity View models