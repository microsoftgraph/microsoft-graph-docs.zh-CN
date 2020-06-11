---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f646f856ed6e3a9714ab900d73a8f2874614e912
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684510"
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
    Values = JToken.Parse("{}"),
    FilterOn = "filterOn-value"
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Columns["{id|name}"].Filter
    .Apply(criteria)
    .Request()
    .PostAsync();

```