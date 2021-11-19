---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e9f2da2a6795837f78ae7cd7f8601251b65dc8b6
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087305"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTimeOff()
userId := "c5d0c76b-80c4-481c-be50-923cd8d680a1"
requestBody.SetUserId(&userId)
sharedTimeOff := msgraphsdk.NewTimeOffItem()
requestBody.SetSharedTimeOff(sharedTimeOff)
sharedTimeOff.SetAdditionalData(map[string]interface{}{
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "white",
}
draftTimeOff := msgraphsdk.NewTimeOffItem()
requestBody.SetDraftTimeOff(draftTimeOff)
draftTimeOff.SetAdditionalData(map[string]interface{}{
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "pink",
}
options := &msgraphsdk.TimesOffRequestBuilderPostOptions{
    Body: requestBody,
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Schedule().TimesOff().Post(options)


```