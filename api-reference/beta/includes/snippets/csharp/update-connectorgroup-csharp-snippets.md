---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 91a4393f76592ce49d2b447e9e612d2bb8f3d5ff
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681152"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectorGroup = new ConnectorGroup
{
    Name = "name-value",
    Region = ConnectorGroupRegion.Nam
};

await graphClient.OnPremisesPublishingProfiles["applicationProxy"].ConnectorGroups["{id}"]
    .Request()
    .UpdateAsync(connectorGroup);

```