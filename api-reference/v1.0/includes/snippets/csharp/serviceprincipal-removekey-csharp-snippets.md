---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6fd6898e70e7e3a5566db12ca98d692e15e34b03
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905375"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var keyId = Guid.Parse("f0b0b335-1d71-4883-8f98-567911bfdca6");

var proof = "eyJ0eXAiOiJ...";

await graphClient.ServicePrincipals["{id}"]
    .RemoveKey(keyId,proof)
    .Request()
    .PostAsync();

```