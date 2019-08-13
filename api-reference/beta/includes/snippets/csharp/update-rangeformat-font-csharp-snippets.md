---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8ec9023bc6984fbe365852bb1ac605777d5f1724
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308860"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFont = new WorkbookRangeFont
{
    Bold = true,
    Color = "#4B180E",
    Size = 26
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["Sheet1"]
    .Range("$A$1").Format.Font
    .Request()
    .UpdateAsync(workbookRangeFont);

```