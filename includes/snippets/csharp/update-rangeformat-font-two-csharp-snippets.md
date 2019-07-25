---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2cd66542b952420c2d1652ad3df1ab175a3961db
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857357"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFont = new WorkbookRangeFont
{
    Italic = true,
    Size = 26
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["Sheet1"]
    .Range('$B$1').Format.Font
    .Request()
    .UpdateAsync(workbookRangeFont);

```