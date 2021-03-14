---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e26c52dbb1881c1d2d512596c2b4c9ffe65a3fa5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800626"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var offerShiftRequest = new OfferShiftRequestObject
{
    SenderShiftId = "SHFT_f7e484ed-fdd6-421c-92d9-0bc9e62e2c29",
    SenderMessage = "Having a family emergency, could you take this shift for me?",
    RecipientUserId = "fe278b61-21ac-4872-8b41-1962bbb98e3c"
};

await graphClient.Teams["{team-id}"].Schedule.OfferShiftRequests
    .Request()
    .Header("Authorization","Bearer {token}")
    .AddAsync(offerShiftRequest);

```