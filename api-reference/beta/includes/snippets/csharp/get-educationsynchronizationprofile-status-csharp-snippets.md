---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d5b65e62689ededb12fe6fb747d7723bdfae1f1fb1b2117f7e5d9fd984d271b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278112"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationSynchronizationProfileStatus = await graphClient.Education.SynchronizationProfiles["{educationSynchronizationProfile-id}"].ProfileStatus
    .Request()
    .GetAsync();

```