---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3020426f8dc11bfa3960fa7c98119b106f58d95a
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61101846"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOfferShiftRequest()
senderShiftId := "SHFT_f7e484ed-fdd6-421c-92d9-0bc9e62e2c29"
requestBody.SetSenderShiftId(&senderShiftId)
senderMessage := "Having a family emergency, could you take this shift for me?"
requestBody.SetSenderMessage(&senderMessage)
recipientUserId := "fe278b61-21ac-4872-8b41-1962bbb98e3c"
requestBody.SetRecipientUserId(&recipientUserId)
headers := map[string]string{
    "Authorization": "Bearer {token}"
}
options := &msgraphsdk.OfferShiftRequestsRequestBuilderPostOptions{
    Body: requestBody,
    H: headers,
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Schedule().OfferShiftRequests().Post(options)


```