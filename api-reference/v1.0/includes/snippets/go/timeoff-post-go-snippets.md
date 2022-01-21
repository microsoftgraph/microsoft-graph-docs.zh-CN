---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7341094fdab2787c18494c15e378d60138175d57
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62110821"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTimeOff()
userId := "c5d0c76b-80c4-481c-be50-923cd8d680a1"
requestBody.SetUserId(&userId)
sharedTimeOff := msgraphsdk.NewTimeOffItem()
requestBody.SetSharedTimeOff(sharedTimeOff)
timeOffReasonId := "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7"
sharedTimeOff.SetTimeOffReasonId(&timeOffReasonId)
startDateTime, err := time.Parse(time.RFC3339, "2019-03-11T07:00:00Z")
sharedTimeOff.SetStartDateTime(&startDateTime)
endDateTime, err := time.Parse(time.RFC3339, "2019-03-12T07:00:00Z")
sharedTimeOff.SetEndDateTime(&endDateTime)
theme := "white"
sharedTimeOff.SetTheme(&theme)
draftTimeOff := msgraphsdk.NewTimeOffItem()
requestBody.SetDraftTimeOff(draftTimeOff)
timeOffReasonId := "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7"
draftTimeOff.SetTimeOffReasonId(&timeOffReasonId)
startDateTime, err := time.Parse(time.RFC3339, "2019-03-11T07:00:00Z")
draftTimeOff.SetStartDateTime(&startDateTime)
endDateTime, err := time.Parse(time.RFC3339, "2019-03-12T07:00:00Z")
draftTimeOff.SetEndDateTime(&endDateTime)
theme := "pink"
draftTimeOff.SetTheme(&theme)
options := &msgraphsdk.TimesOffRequestBuilderPostOptions{
    Body: requestBody,
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Schedule().TimesOff().Post(options)


```