---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a02ac3ce357f3e2fd18559c5b18ce2179018c0a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809282"
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

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"]
    .Request()
    .UpdateAsync(workbookTable);

```