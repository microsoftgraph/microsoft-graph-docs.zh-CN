---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 919c097ee602309421d10a2b0a7779572f68da80169078ae5960681b707fa713
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161773"
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

var method = "method-value";

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Sort
    .Apply(matchCase,method,fields)
    .Request()
    .PostAsync();

```