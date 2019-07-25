---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 64fd80e19e377e51123ac066f4369960e4246cc6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724595"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookTableRow = new WorkbookTableRow
{
    Index = 99,
    Values = "values-value"
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Rows["{index}"]
    .Request()
    .UpdateAsync(workbookTableRow);

```