---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c3ec4a4ffcb743e25eda2c8042d51f9875b08c25aafee76554f413d170b9cd5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277700"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.B2xUserFlows["{b2xIdentityUserFlow-id}"].IdentityProviders["{identityProvider-id}"].Reference
    .Request()
    .DeleteAsync();

```