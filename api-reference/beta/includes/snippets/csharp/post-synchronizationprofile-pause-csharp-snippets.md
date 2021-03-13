---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1fa6b9166f90264258a4fbcd8ab2f4c2c8d04750
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803812"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.SynchronizationProfiles["{educationSynchronizationProfile-id}"]
    .Pause()
    .Request()
    .PostAsync();

```