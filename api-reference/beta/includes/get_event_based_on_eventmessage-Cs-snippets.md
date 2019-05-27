---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8732a356ca1dc70696960d8a4eab099eb6cc1385
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34471443"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = await graphClient.Me.Messages["AAMkADYAAAImV_jAAA="]
    .Request()
    .Expand("eventMessage/event")
    .GetAsync();

```