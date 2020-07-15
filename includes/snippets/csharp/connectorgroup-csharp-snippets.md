---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9999bb72155b842c3362f4479ab3b9fa53987472
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142352"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectorGroup = new ConnectorGroup
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/onPremisesPublishingProfiles/applicationproxy/connectorGroups/3e6f4c35-a04b-4d03-b98a-66fff89b72e6"}
    }
};

await graphClient.Applications["bf21f7e9-9d25-4da2-82ab-7fdd85049f83"].ConnectorGroup.Reference
    .Request()
    .PutAsync(connectorGroup);

```