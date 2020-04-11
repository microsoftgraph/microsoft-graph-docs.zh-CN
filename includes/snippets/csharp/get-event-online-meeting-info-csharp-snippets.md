---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f43063f6b09154fe3a39d677dbdba0c17949ccd
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636959"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @event = await graphClient.Me.Events["AAMkADAGu0AABIGYDZAAA="]
    .Request()
    .Select( e => new {
             e.IsOnlineMeeting,
             e.OnlineMeetingProvider,
             e.OnlineMeeting 
             })
    .GetAsync();

```