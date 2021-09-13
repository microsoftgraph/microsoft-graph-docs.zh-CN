---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 628afdea2ebd80e241ab5699ac49425947c866d5994dd749fa94732a3fab3530
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215986"
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