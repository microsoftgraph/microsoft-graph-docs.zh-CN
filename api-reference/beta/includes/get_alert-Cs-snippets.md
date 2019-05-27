---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d4df16ee11685a1b4d429214ba577f4c26eef537
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474154"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var alert = await graphClient.Security.Alerts["{id}"]
    .Request()
    .GetAsync();

```