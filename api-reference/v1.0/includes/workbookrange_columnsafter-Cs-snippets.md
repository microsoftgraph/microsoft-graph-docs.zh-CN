---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 55f405accec5760888991c8693d4dfe13ed7e3f4
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34462325"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Root.Workbook.Worksheets["{id}"]
    .Range()
    .ColumnsAfter(count)
    .Request()
    .PostAsync();

```