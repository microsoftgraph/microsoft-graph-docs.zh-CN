---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1e69a21c3d822d8b76b2c70dc25f28f079689309b3e71c75ffce1566e1714f9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54240506"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @event = new Event
{
    IsOnlineMeeting = true,
    OnlineMeetingProvider = OnlineMeetingProviderType.TeamsForBusiness
};

await graphClient.Me.Events["AAMkADAGu0AABIGYDaAAA="]
    .Request()
    .UpdateAsync(@event);

```