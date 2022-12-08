---
Order: 20
Title: Features
Description: Features of the Cake.Issues.DupFinder addin.
---
The [Cake.Issues.DupFinder addin] provides the following features:

# Basic features

* Reads code duplicates from [JetBrains dupFinder] log files.
* For every duplicate fragment a separate issue is created.

# Supported IIssue properties

|                                                                    | Property                          | Remarks                          |
|--------------------------------------------------------------------|-----------------------------------|----------------------------------|
| <span class="glyphicon glyphicon-ok" style="color:green"></span>   | `IIssue.ProviderType`             |                                  |
| <span class="glyphicon glyphicon-ok" style="color:green"></span>   | `IIssue.ProviderName`             |                                  |
| <span class="glyphicon glyphicon-ok" style="color:green"></span>   | `IIssue.Run`                      | Can be set while reading issues  |
| <span class="glyphicon glyphicon-ok" style="color:green"></span>   | `IIssue.Identifier`               |                                  |
| <span class="glyphicon glyphicon-remove" style="color:red"></span> | `IIssue.ProjectName`              |                                  |
| <span class="glyphicon glyphicon-remove" style="color:red"></span> | `IIssue.ProjectFileRelativePath`  |                                  |
| <span class="glyphicon glyphicon-ok" style="color:green"></span>   | `IIssue.AffectedFileRelativePath` |                                  |
| <span class="glyphicon glyphicon-ok" style="color:green"></span>   | `IIssue.Line`                     |                                  |
| <span class="glyphicon glyphicon-ok" style="color:green"></span>   | `IIssue.EndLine`                  |                                  |
| <span class="glyphicon glyphicon-remove" style="color:red"></span> | `IIssue.Column`                   |                                  |
| <span class="glyphicon glyphicon-remove" style="color:red"></span> | `IIssue.EndColumn`                |                                  |
| <span class="glyphicon glyphicon-ok" style="color:green"></span>   | `IIssue.MessageText`              |                                  |
| <span class="glyphicon glyphicon-ok" style="color:green"></span>   | `IIssue.MessageHtml`              |                                  |
| <span class="glyphicon glyphicon-ok" style="color:green"></span>   | `IIssue.MessageMarkdown`          |                                  |
| <span class="glyphicon glyphicon-ok" style="color:green"></span>   | `IIssue.Priority`                 | Always [IssuePriority.Warning]   |
| <span class="glyphicon glyphicon-ok" style="color:green"></span>   | `IIssue.PriorityName`             | Always `Warning`                 |
| <span class="glyphicon glyphicon-ok" style="color:green"></span>   | `IIssue.Rule`                     | Always `dupFinder`               |
| <span class="glyphicon glyphicon-remove" style="color:red"></span> | `IIssue.RuleUrl`                  |                                  |

## Additional information

The following values are provided in the [IIssue.AdditionalInformation] property:

| Key    | Description                                                                      |
|--------|----------------------------------------------------------------------------------|
| `cost` | Cost of the duplicate. The bigger the duplicated code block the higher the cost. |

[JetBrains dupFinder]: https://www.jetbrains.com/help/resharper/dupFinder.html
[Cake.Issues.DupFinder addin]: https://www.nuget.org/packages/Cake.Issues.DupFinder
[IIssue.AdditionalInformation]: /api/Cake.Issues/IIssue/FE50CEF3
