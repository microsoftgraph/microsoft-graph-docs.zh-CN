---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ac3fd8c539e2021523a3349c39cbdb8109722d2b
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329427"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var b2xUserFlows = await graphClient.Identity.B2xUserFlows
    .Request()
    .GetAsync();

```