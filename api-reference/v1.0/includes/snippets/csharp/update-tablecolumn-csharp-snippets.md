---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 908edefb78e9641228c905f968a50f04b84259229b00ac1bda5d6f6e7f4f747d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378696"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookTableColumn = new WorkbookTableColumn
{
    Name = "name-value",
    Index = 99,
    Values = JsonDocument.Parse(@"""values-value""")
};

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Columns["{workbookTableColumn-id}"]
    .Request()
    .UpdateAsync(workbookTableColumn);

```