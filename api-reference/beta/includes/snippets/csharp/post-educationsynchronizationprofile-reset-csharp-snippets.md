---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 19cb9ac72b270cafd389adc8678127d45f6bba80
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791075"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.SynchronizationProfiles["{educationSynchronizationProfile-id}"]
    .Reset()
    .Request()
    .PostAsync();

```