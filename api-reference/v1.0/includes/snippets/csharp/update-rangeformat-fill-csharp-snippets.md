---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e038c21644755f066fd5e433295f5c9a66c845f7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891993"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFill = new WorkbookRangeFill
{
    Color = "#FF0000"
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{sheet-id}"]
    .Range('$A$1').Format.Fill
    .Request()
    .UpdateAsync(workbookRangeFill);

```