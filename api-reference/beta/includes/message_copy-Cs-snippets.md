---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 97ec46bb649c0cb899245cd336dbb8e08e374bfc
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444179"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var destinationId = "destinationId-value";

await graphClient.Me.Messages["{id}"]
    .Copy(destinationId)
    .Request()
    .PostAsync();

```