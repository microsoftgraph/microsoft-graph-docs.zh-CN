---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b7349b188e38e1a153da6e3f29593ad560323c77ed026ffec7e86ef61a4f2fe8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106908"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.SynchronizationProfiles["{educationSynchronizationProfile-id}"]
    .Pause()
    .Request()
    .PostAsync();

```