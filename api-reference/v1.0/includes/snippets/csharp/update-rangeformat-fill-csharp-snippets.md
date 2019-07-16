---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 739d0db0868cc3098be9e538900a031e99b3d135
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35737738"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFill = new WorkbookRangeFill
{
    Color = "#FF0000"
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{sheet-id}"].Range('$A$1').Format.Fill
    .Request()
    .UpdateAsync(workbookRangeFill);

```