---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 470409eed1ebe085ca1a08926829314e6e1fb197
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802179"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.SynchronizationProfiles["{educationSynchronizationProfile-id}"]
    .Start()
    .Request()
    .PostAsync();

```