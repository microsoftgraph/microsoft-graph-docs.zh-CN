---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2af75dc5564daf23cba0772ea45bdb858d2c5a3c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784601"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{servicePrincipal-id}"].Owners["{directoryObject-id}"].Reference
    .Request()
    .DeleteAsync();

```