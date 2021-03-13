---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce3e7dc003e7d51fe1ab2620e9ec9413d5a4c67c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773520"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onlineMeeting = new OnlineMeeting
{
    StartDateTime = DateTimeOffset.Parse("2020-09-09T21:33:30.8546353+00:00"),
    EndDateTime = DateTimeOffset.Parse("2020-09-09T22:03:30.8566356+00:00"),
    Subject = "Patch Meeting Subject"
};

await graphClient.Me.OnlineMeetings["{onlineMeeting-id}"]
    .Request()
    .UpdateAsync(onlineMeeting);

```