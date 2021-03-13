---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e516ad2c837f07d4af6fa444f531a2887698d2f4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782040"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationSynchronizationProfileStatus = await graphClient.Education.SynchronizationProfiles["{educationSynchronizationProfile-id}"].ProfileStatus
    .Request()
    .GetAsync();

```