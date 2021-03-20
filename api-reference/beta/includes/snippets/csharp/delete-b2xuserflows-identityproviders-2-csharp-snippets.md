---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7f95be9e20f2265c40539c499778941b7c8110c9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944590"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.B2xUserFlows["{b2xIdentityUserFlow-id}"].IdentityProviders["{identityProvider-id}"].Reference
    .Request()
    .DeleteAsync();

```