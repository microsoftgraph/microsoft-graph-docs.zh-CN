---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 26231dd5a2fe78a46710e7390ef7710c9b404f24
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66438651"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userSource = new Microsoft.Graph.Security.UserSource
{
    Email = "admin@M365x809305.onmicrosoft.com",
    IncludedSources = Microsoft.Graph.Security.SourceType.Mailbox | Microsoft.Graph.Security.SourceType.Site
};

await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].LegalHolds["{security.ediscoveryHoldPolicy-id}"].UserSources
    .Request()
    .AddAsync(userSource);

```