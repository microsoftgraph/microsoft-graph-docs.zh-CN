---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d020b4337aeb38f62a6982f60cc52ab00cb8bd32
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329546"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.B2xUserFlows["B2X_1_PartnerSignUp"].IdentityProviders["Facebook-OAUTH"].Reference
    .Request()
    .DeleteAsync();

```