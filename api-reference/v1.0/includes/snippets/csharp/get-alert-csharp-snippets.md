---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc53ce0096a427fa206fde6689962953a5a673f4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804856"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var alert = await graphClient.Security.Alerts["{alert-id}"]
    .Request()
    .GetAsync();

```