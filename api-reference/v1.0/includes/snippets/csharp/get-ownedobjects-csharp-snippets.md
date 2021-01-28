---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 31fbac4832f3ebacf87ec9113eb10ca3a93dabdf
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015740"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ownedObjects = await graphClient.ServicePrincipals["{id}"].OwnedObjects
    .Request()
    .GetAsync();

```