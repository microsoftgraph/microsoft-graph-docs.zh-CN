---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5352d810c039cca722fc6da63275b2a7debe3c6d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874256"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFill = new WorkbookRangeFill
{
    Color = "#0000FF"
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["Sheet1"]
    .Range('$C$1').Format.Fill
    .Request()
    .UpdateAsync(workbookRangeFill);

```