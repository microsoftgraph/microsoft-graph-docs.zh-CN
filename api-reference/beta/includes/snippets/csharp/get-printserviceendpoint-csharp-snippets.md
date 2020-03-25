---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b89a2dea8201ba3f1748e5ffbe686fd97c15c8e3
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947513"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printServiceEndpoint = await graphClient.Print.Services["{id}"].Endpoints["{name}"]
    .Request()
    .GetAsync();

```