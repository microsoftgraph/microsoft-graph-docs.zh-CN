---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fb4fd2977a1489975a053f29b201a26bc9a40525
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723700"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookPivotTable = await graphClient.Drive.Root.Workbook.Worksheets["{id}"].PivotTables["{id}"]
    .Request()
    .GetAsync();

```