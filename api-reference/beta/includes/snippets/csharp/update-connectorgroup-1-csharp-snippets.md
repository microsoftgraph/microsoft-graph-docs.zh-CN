---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72089d44cc14ae89e7a705708c56f20b6f41d8446420665dfc79f2b3c2f2ff11
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158306"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectorGroup = new ConnectorGroup
{
    Name = "Connector Group Demo"
};

await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"].ConnectorGroups
    .Request()
    .AddAsync(connectorGroup);

```