---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c508bd277a0e8a026dc3d116d9f650cffa77d31d890f16169017c06ead6c4267
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164102"
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