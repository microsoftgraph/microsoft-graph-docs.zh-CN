---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4836a938651f5966ea13e3a4fc49d06ffc89cc77
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636964"
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