---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b134c667624c83e602c1f4004d21be976ae3d03c
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66096130"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ediscoveryHoldPolicy = new Microsoft.Graph.Security.EdiscoveryHoldPolicy
{
    Displayname = "My legalHold with sources",
    Description = "Created from Graph API",
    ContentQuery = "Bazooka",
    AdditionalData = new Dictionary<string, object>()
    {
        {"userSources@odata.bind", "[{\"@odata.type\":\"microsoft.graph.security.userSource\",\"email\":\"SalesTeam@M365x809305.OnMicrosoft.com\"}]"},
        {"siteSources@odata.bind", "[{\"@odata.type\":\"microsoft.graph.security.siteSource\",\"site\":{\"webUrl\":\"https://m365x809305.sharepoint.com/sites/Design-topsecret\"}}]"}
    }
};

await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].LegalHolds
    .Request()
    .AddAsync(ediscoveryHoldPolicy);

```