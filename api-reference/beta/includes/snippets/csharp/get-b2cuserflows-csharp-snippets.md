---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c3a28b8ba4b6127fbc5dcc70daff294da3ca6ea
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329750"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var b2cIdentityUserFlow = await graphClient.Identity.B2cUserFlows["{id}"]
    .Request()
    .GetAsync();

```