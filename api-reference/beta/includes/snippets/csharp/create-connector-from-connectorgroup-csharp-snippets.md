---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 383f777adff894b0e57e50b133eabc2b5fb8226e
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681180"
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

await graphClient.OnPremisesPublishingProfiles["applicationProxy"].ConnectorGroups["{id}"].Members.References
    .Request()
    .AddAsync(connector);

```