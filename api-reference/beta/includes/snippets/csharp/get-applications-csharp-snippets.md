---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1bac25bc45062c40f4c3edcfda0f3d397c524929
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681404"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var applications = await graphClient.OnPremisesPublishingProfiles["applicationProxy"].ConnectorGroups["{id}"].Applications
    .Request()
    .GetAsync();

```