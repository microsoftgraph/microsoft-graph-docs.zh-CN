---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2617e692e8d3fd405ed00b169c397686e9611da0
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739940"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookTableColumn = new WorkbookTableColumn
{
    Name = "name-value",
    Index = 99,
    Values = "values-value"
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Columns["{id|name}"]
    .Request()
    .UpdateAsync(workbookTableColumn);

```