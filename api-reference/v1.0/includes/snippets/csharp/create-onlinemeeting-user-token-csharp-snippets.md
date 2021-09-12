---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f649fd3358ddc6cff22b996bd6b6ead70d23f871bfdfb99d1cc405c8bf989ea9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278720"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onlineMeeting = new OnlineMeeting
{
    StartDateTime = DateTimeOffset.Parse("2019-07-12T21:30:34.2444915+00:00"),
    EndDateTime = DateTimeOffset.Parse("2019-07-12T22:00:34.2464912+00:00"),
    Subject = "User Token Meeting"
};

await graphClient.Me.OnlineMeetings
    .Request()
    .AddAsync(onlineMeeting);

```