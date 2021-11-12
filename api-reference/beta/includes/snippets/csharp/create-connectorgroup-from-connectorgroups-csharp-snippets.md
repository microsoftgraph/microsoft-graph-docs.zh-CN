---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 10e206d3e5b963b6741c86e82a84fc84c5647ac2eab49043679263fd1cf2e977
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902512"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectorGroup = new ConnectorGroup
{
    Name = "name-value",
    IsDefault = false
};

await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"].ConnectorGroups
    .Request()
    .AddAsync(connectorGroup);

```