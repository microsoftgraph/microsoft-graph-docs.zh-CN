---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6b3037e8a7f3143ebaae1864336e01fe1fe142f0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34448927"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = await graphClient.Me.Messages["AQMkADJmMTUAAAgVZAAAA"]
    .Request()
    .Expand("mentions")
    .GetAsync();

```