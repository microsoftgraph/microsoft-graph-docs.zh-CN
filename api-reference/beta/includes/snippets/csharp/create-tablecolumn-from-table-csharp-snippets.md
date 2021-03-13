---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b43f360c42a50258be85d236d575e2fdf8c9242d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788228"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookTableColumn = new WorkbookTableColumn
{
    Id = "99",
    Name = "name-value",
    Index = 99,
    Values = "values-value"
};

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Columns
    .Request()
    .AddAsync(workbookTableColumn);

```