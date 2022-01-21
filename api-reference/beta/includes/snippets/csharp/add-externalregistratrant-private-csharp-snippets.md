---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7f01da436f19dcb39110ab52c2fcffc59f4d0ea6
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62118897"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var meetingRegistrantBase = new ExternalMeetingRegistrant
{
    Id = "30494ab7-7338-4592-bfec-a4333be2a0a6",
    TenantId = "909c6581-5130-43e9-88f3-fcb3582cde37",
    UserId = "cc515404-b55c-466e-b896-992c918ecc01"
};

await graphClient.Me.OnlineMeetings["{onlineMeeting-id}"].Registration.Registrants
    .Request()
    .AddAsync(meetingRegistrantBase);

```