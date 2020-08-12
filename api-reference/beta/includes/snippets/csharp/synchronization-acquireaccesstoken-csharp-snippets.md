---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e4861308a3a430d797ccb2541188ea72fe9b1e3a
ms.sourcegitcommit: 8e18d7fe3c869b2fd48872365116175d3bdce1b7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/12/2020
ms.locfileid: "46643745"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var credentials = new List<SynchronizationSecretKeyStringValuePair>()
{
    new SynchronizationSecretKeyStringValuePair
    {
    }
};

await graphClient.Applications["{applicationsId}"].Synchronization
    .AcquireAccessToken(credentials)
    .Request()
    .PostAsync();

```