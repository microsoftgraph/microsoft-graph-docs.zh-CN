---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 92c4ff66862c4cb36630a58cacea89f3a1aec5a5
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098777"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewShift()
id := "SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8"
requestBody.SetId(&id)
userId := "c5d0c76b-80c4-481c-be50-923cd8d680a1"
requestBody.SetUserId(&userId)
schedulingGroupId := "TAG_228940ed-ff84-4e25-b129-1b395cf78be0"
requestBody.SetSchedulingGroupId(&schedulingGroupId)
sharedShift := msgraphsdk.NewShiftItem()
requestBody.SetSharedShift(sharedShift)
displayName := "Day shift"
sharedShift.SetDisplayName(&displayName)
notes := "Please do inventory as part of your shift."
sharedShift.SetNotes(&notes)
startDateTime, err := time.Parse(time.RFC3339, "2019-03-11T15:00:00Z")
sharedShift.SetStartDateTime(&startDateTime)
endDateTime, err := time.Parse(time.RFC3339, "2019-03-12T00:00:00Z")
sharedShift.SetEndDateTime(&endDateTime)
theme := "blue"
sharedShift.SetTheme(&theme)
sharedShift.SetActivities( []ShiftActivity {
    msgraphsdk.NewShiftActivity(),
isPaid := true
    SetIsPaid(&isPaid)
startDateTime, err := time.Parse(time.RFC3339, "2019-03-11T15:00:00Z")
    SetStartDateTime(&startDateTime)
endDateTime, err := time.Parse(time.RFC3339, "2019-03-11T15:15:00Z")
    SetEndDateTime(&endDateTime)
code := ""
    SetCode(&code)
displayName := "Lunch"
    SetDisplayName(&displayName)
}
draftShift := msgraphsdk.NewShiftItem()
requestBody.SetDraftShift(draftShift)
displayName := "Day shift"
draftShift.SetDisplayName(&displayName)
notes := "Please do inventory as part of your shift."
draftShift.SetNotes(&notes)
startDateTime, err := time.Parse(time.RFC3339, "2019-03-11T15:00:00Z")
draftShift.SetStartDateTime(&startDateTime)
endDateTime, err := time.Parse(time.RFC3339, "2019-03-12T00:00:00Z")
draftShift.SetEndDateTime(&endDateTime)
theme := "blue"
draftShift.SetTheme(&theme)
draftShift.SetActivities( []ShiftActivity {
    msgraphsdk.NewShiftActivity(),
isPaid := true
    SetIsPaid(&isPaid)
startDateTime, err := time.Parse(time.RFC3339, "2019-03-11T15:00:00Z")
    SetStartDateTime(&startDateTime)
endDateTime, err := time.Parse(time.RFC3339, "2019-03-11T15:30:00Z")
    SetEndDateTime(&endDateTime)
code := ""
    SetCode(&code)
displayName := "Lunch"
    SetDisplayName(&displayName)
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Schedule().Shifts().Post(requestBody)


```