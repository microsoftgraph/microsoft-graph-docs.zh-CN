---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 264d40763ab0cf8f1305516b77091039f4b09ef2
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945279"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectorGroup = new ConnectorGroup
{
    Name = "Connector Group Demo"
};

await graphClient.OnPremisesPublishingProfiles["applicationProxy"].ConnectorGroups
    .Request()
    .AddAsync(connectorGroup);

```