---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fb63360d8e861bd04b95e542367ce92001f7ee32
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734901"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookTable = new WorkbookTable
{
    Name = "name-value",
    ShowHeaders = true,
    ShowTotals = true,
    Style = "style-value"
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"]
    .Request()
    .UpdateAsync(workbookTable);

```