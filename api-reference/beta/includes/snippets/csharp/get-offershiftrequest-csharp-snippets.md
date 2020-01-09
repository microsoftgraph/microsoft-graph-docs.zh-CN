---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c35596222b0e61bfda2c285403fa056d455dcb21
ms.sourcegitcommit: 66c8fcafee151278f8089cd26d0c5766d33d04a8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/09/2020
ms.locfileid: "40994830"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var offerShiftRequest = new OfferShiftRequest
{
    SenderShiftId = "SHFT_f7e484ed-fdd6-421c-92d9-0bc9e62e2c29",
    SenderMessage = "Having a family emergency, could you take this shift for me?",
    RecipientUserId = "fe278b61-21ac-4872-8b41-1962bbb98e3c"
};

await graphClient.Teams["788b75d2-a911-48c0-a5e2-dc98480457e3"].Schedule.OfferShiftRequests
    .Request()
    .Header("Authorization","Bearer {token}")
    .AddAsync(offerShiftRequest);

```