---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20ff9a32a90a9d8949d03a009511dc95c05b563f
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44683983"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var offerShiftRequest = new OfferShiftRequestObject
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