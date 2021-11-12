---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 695fac52b99a69c5454c2fb68e1c5bbffd8eb7bc053f2cad335b65cfa431d47b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162217"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var criteria = new WorkbookFilterCriteria
{
    Criterion1 = "criterion1-value",
    Criterion2 = "criterion2-value",
    Color = "color-value",
    Operator = "",
    Icon = new WorkbookIcon
    {
        Set = "set-value",
        Index = 99
    },
    DynamicCriteria = "dynamicCriteria-value",
    Values = JsonDocument.Parse("{}"),
    FilterOn = "filterOn-value"
};

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Columns["{workbookTableColumn-id}"].Filter
    .Apply(criteria)
    .Request()
    .PostAsync();

```