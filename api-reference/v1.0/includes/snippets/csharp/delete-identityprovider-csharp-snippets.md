---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b62f699c134b5f16369ca341d35b19968bdd7c11
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53579841"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.IdentityProviders["{identityProviderBase-id}"]
    .Request()
    .DeleteAsync();

```