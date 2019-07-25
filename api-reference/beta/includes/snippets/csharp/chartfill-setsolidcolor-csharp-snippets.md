---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 65cf70a7b0b2277e217ba9857f0806c2f8c8822b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708179"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var color = "color-value";

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Format.Fill
    .SetSolidColor(color)
    .Request()
    .PostAsync();

```