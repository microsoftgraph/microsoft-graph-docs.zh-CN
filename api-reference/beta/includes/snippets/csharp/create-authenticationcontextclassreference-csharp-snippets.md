---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bea867ee17d81bd6363995930c6ad3b656199635
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52663942"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authenticationContextClassReference = new AuthenticationContextClassReference
{
    Id = "c1",
    DisplayName = "Contoso medium",
    Description = "Medium protection level defined for Contoso policy",
    IsAvailable = true
};

await graphClient.Identity.ConditionalAccess.AuthenticationContextClassReferences
    .Request()
    .AddAsync(authenticationContextClassReference);

```