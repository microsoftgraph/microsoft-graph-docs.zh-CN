---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 93f29fa2451441f78b5776b0a9ee831de27a8126
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35737323"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Format.Fill
    .Clear()
    .Request()
    .PostAsync();

```