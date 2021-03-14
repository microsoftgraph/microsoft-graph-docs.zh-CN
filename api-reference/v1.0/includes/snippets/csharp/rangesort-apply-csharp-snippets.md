---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9fc2ddf4559c0309019cadaffab8c998cac9ff1c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785261"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var fields = new List<WorkbookSortField>()
{
    new WorkbookSortField
    {
        Key = 99,
        SortOn = "sortOn-value",
        Ascending = true,
        Color = "color-value",
        DataOption = "dataOption-value",
        Icon = new WorkbookIcon
        {
            Set = "set-value",
            Index = 99
        }
    }
};

var matchCase = true;

var hasHeaders = true;

var orientation = "orientation-value";

var method = "method-value";

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range().Sort
    .Apply(matchCase,hasHeaders,orientation,method,fields)
    .Request()
    .PostAsync();

```