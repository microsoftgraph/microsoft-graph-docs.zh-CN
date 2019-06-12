---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fc1618d032493ea678eda8cb81d7f15e9c91a8f5
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34843603"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFill = new WorkbookRangeFill
{
    Color = "#0000FF"
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["Sheet1"].Range('$C$1').Format.Fill
    .Request()
    .UpdateAsync(workbookRangeFill);

```