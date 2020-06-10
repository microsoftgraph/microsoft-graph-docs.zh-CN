---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a0662b446a83efd30838be6503d22e8f7092151b
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681320"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectorGroups = await graphClient.OnPremisesPublishingProfiles["applicationProxy"].ConnectorGroups
    .Request()
    .GetAsync();

```