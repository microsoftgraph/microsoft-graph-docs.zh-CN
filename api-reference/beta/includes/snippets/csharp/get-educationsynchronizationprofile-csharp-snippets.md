---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b57930ce3e5ba56e55b87deed9a6ed029c337059
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803249"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationSynchronizationProfile = await graphClient.Education.SynchronizationProfiles["{educationSynchronizationProfile-id}"]
    .Request()
    .GetAsync();

```