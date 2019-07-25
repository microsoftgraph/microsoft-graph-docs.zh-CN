---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8d578ef84b324ecb5453c3c418734fe51431258f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723692"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Drive.Root.Workbook.Worksheets["{id}"]
    .Range()
    .ColumnsBefore(count)
    .Request()
    .PostAsync();

```