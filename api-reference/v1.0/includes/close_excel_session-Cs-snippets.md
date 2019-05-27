---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d3460289049e51b40b6b03984ddc6a8db7a0d335
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34467042"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook
    .CloseSession(this)
    .Request()
    .Header("workbook-session-id","{session-id}")
    .PostAsync();

```