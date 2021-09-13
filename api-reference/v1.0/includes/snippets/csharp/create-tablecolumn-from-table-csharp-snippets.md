---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d68d08c73ddd60b7a0184660423715444f2eb838f99d248f06483ece58c16d64
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219991"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookTableColumn = new WorkbookTableColumn
{
    Id = "99",
    Name = "name-value",
    Index = 99,
    Values = JsonDocument.Parse(@"""values-value""")
};

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Columns
    .Request()
    .AddAsync(workbookTableColumn);

```