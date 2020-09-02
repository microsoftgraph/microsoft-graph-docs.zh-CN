---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6390ce0412cb0389f0373eea3d9a78897c9fdd22
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329390"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.B2xUserFlows["{id}"]
    .Request()
    .DeleteAsync();

```