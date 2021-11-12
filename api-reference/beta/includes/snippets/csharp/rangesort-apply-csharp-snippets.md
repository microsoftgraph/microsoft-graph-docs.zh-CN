---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 34b202315869f720e300d7df9a47dcd5699067592bc82eb5dd83e63dff653a76
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333438"
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