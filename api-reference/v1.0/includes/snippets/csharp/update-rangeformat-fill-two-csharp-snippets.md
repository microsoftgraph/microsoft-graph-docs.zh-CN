---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f84b58f2018b5309a970b17a728e0aa0b8f7643c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36324760"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFill = new WorkbookRangeFill
{
    Color = "#00FF00"
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{sheet-id}"]
    .Range("$B$1").Format.Fill
    .Request()
    .UpdateAsync(workbookRangeFill);

```