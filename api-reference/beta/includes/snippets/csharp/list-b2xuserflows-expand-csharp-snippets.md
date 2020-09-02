---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 75ed3faa0b923c5dc3de681eb220ea6b6293e576
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329424"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var b2xUserFlows = await graphClient.Identity.B2xUserFlows
    .Request()
    .Expand("identityProviders")
    .GetAsync();

```