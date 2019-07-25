---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6b3037e8a7f3143ebaae1864336e01fe1fe142f0
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35729811"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = await graphClient.Me.Messages["AQMkADJmMTUAAAgVZAAAA"]
    .Request()
    .Expand("mentions")
    .GetAsync();

```