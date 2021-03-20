---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc52a934c8a2922845a48dc6552c50400a04b45f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944869"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"].IdentityProviders["{identityProvider-id}"].Reference
    .Request()
    .DeleteAsync();

```