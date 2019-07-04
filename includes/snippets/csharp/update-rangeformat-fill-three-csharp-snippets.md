---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fc1618d032493ea678eda8cb81d7f15e9c91a8f5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35533261"
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