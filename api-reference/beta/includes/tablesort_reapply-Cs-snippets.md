---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8e7f0b5f8e09c5a2a5f1dd944cb6bcdb17c15287
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34457423"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Sort
    .Reapply()
    .Request()
    .PostAsync();

```