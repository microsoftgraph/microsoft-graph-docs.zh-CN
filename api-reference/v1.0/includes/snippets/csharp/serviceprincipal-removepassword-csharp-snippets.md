---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6db8a9f8506c8767461982868e04dc8ec794ee29
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785053"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var keyId = Guid.Parse("f0b0b335-1d71-4883-8f98-567911bfdca6");

await graphClient.ServicePrincipals["{servicePrincipal-id}"]
    .RemovePassword(keyId)
    .Request()
    .PostAsync();

```