# Errata, Improvements and Troubleshooting

If you find any mistakes in the sixth edition, *C# 10 and .NET 6 - Modern Cross-Platform Development*, or if you have suggestions for improvements, then please [raise an issue in this repository](https://github.com/markjprice/cs10dotnet6/issues) or email me at markjprice (at) gmail.com.



## Page 18 - Writing code using Visual Studio 2022

In Step 3, the project template name has been changed from **Console Application** to **Console App** in the final release of Visual Studio 2022, as shown in the following screenshot:

![Project template Console Application is now Console App](images/console-app-template.png)

## Page 25 - Writing code using Visual Studio Code

In Step 14, I say that the first time you open a code file, Visual Studio Code may have to download and install C# dependencies and so on. This will not happen if you do not trust the workspace. 

At the top of the window, in the blue bar, click **Manage**, as shown in the following screenshot:

![Restricted mode blue bar](images/restricted-mode.png)


Click the **Trust** button, as shown in the following screenshot:

![Restricted mode](images/restricted-mode-2.png)

You will then trust the workspace and extensions will activate as described in the book. 

![A trusted workspace allows extensions to run](images/trust-workspace.png)

## Page 87 - Passing arguments to a console app

In Step 5, I say, "If you are using Visual Studio, then navigate to **Project** | **Arguments Properties**, select the **Debug** tab, and in the **Application arguments** box, enter some arguments". 

Microsoft changed the user interface of Visual Studio 2022 after that step was written. 

It should now say, "If you are using Visual Studio, then navigate to **Project** | **Arguments Properties**, select 
the **Debug** tab, click **Open debug launch profiles UI**, and in the **Command line arguments** box, enter some arguments", as shown in the following screenshot:

![Updated UI for setting arguments in Visual Studio 2022](images/erratum-page-87a.png)

In *Figure 2.6*, it is difficult to see the hyphen in the second argument in the PDF edition (shown in the screenshot below) and impossible to see it in the Kindle edition. 

In Step 5, it would have been clearer if I had written out the arguments as I did in Step 6 instead of relying on Amazon's image processing to clearly show the hyphen! 

For example, `firstarg second-arg third:arg "fourth arg"`. 

![Barely visible hyphen in second-arg](images/erratum-page-87b.png)

## Page 92 - Exercise 2.3 – Practice number sizes and ranges

In Exercise 2.3, I say, "create a console application project named Exercise02". I should have said, "create a console application project named Exercise03".

<!---
## Conflicting build servers for Omnisharp with Visual Studio Code

If you have Visual Studio for Windows and Visual Studio Code and the C# extension installed on the same computer, the build process can sometimes conflict. This is because Visual Studio has its own non-standard build server that is different from the standard build server used by .NET SDK and Omnisharp.

You can determine if you have this issue by reviewing the Omnisharp logs. 

For example, as shown in the following output:
```
TODO
```

You can control where Omnisharp looks for the build server by creating a configuration file. 

1. In the installation folder for Omnisharp: xxx
2. Create a file named omnisharp.json.
3. Contents of the file:
```
TODO
```
Read more about this issue: https://github.com/OmniSharp/omnisharp-roslyn/wiki/Configuration-Options
--->
