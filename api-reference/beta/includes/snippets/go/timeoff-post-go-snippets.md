---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3edf5a962307a9dd9c91dda12bdb574bf865ef11
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326873"
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
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Schedule().TimesOff().Post(requestBody)


```