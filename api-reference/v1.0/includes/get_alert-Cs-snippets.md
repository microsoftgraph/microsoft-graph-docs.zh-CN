---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e0984a84a80c562a3635df91130665d05c7b9566
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34470025"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var alert = await graphClient.Security.Alerts["{alert_id}"]
    .Request()
    .GetAsync();

```