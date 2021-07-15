---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 97fb9787442d66b7d6a1c1e0f7cf4e59d9620094
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439654"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"].UserFlowIdentityProviders["{identityProviderBase-id}"].Reference
    .Request()
    .DeleteAsync();

```