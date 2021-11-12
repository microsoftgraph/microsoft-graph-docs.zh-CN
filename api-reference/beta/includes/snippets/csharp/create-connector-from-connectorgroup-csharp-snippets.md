---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 676c63d183558a31c14a2819bc224215691a429f1b71ebac10aff10ad269d5ec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101411"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connector = new Connector
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/{id}"}
    }
};

await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"].ConnectorGroups["{connectorGroup-id}"].Members.References
    .Request()
    .AddAsync(connector);

```