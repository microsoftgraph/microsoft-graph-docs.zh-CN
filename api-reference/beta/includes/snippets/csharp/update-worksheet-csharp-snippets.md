---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a6187c0d78ba5b7abb601b3c8fbabcbfda75c1d5
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723588"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookWorksheet = new WorkbookWorksheet
{
    Position = 99,
    Name = "name-value",
    Visibility = "visibility-value"
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"]
    .Request()
    .UpdateAsync(workbookWorksheet);

```