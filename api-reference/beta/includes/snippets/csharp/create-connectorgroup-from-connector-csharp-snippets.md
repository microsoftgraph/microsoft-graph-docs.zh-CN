---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 25f414a8880355fd2c2951d7e31d99a4f89c71ba
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49752986"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectorGroup = new ConnectorGroup
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}"}
    }
};

await graphClient.OnPremisesPublishingProfiles["applicationProxy"].Connectors["{id}"].MemberOf.References
    .Request()
    .AddAsync(connectorGroup);

```