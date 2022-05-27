---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0bb831c2c245b260e57ba2bd5f8c98a782cd4f76
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65719203"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectorGroupReference = new ReferenceRequestBody
{
    ODataId = "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}"
};

await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"].Connectors["{connector-id}"].MemberOf.References
    .Request()
    .AddAsync(connectorGroupReference);

```