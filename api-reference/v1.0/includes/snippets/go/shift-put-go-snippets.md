---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 62b7164bcec47a751925fdf7904f702c6fb4d772
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131990"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewShift()
id := "SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8"
requestBody.SetId(&id)
createdDateTime, err := time.Parse(time.RFC3339, "2019-03-14T04:32:51.451Z")
requestBody.SetCreatedDateTime(&createdDateTime)
lastModifiedDateTime, err := time.Parse(time.RFC3339, "2019-03-14T05:32:51.451Z")
requestBody.SetLastModifiedDateTime(&lastModifiedDateTime)
userId := "c5d0c76b-80c4-481c-be50-923cd8d680a1"
requestBody.SetUserId(&userId)
schedulingGroupId := "TAG_228940ed-ff84-4e25-b129-1b395cf78be0"
requestBody.SetSchedulingGroupId(&schedulingGroupId)
lastModifiedBy := msgraphsdk.NewIdentitySet()
requestBody.SetLastModifiedBy(lastModifiedBy)
lastModifiedBy.SetApplication(nil)
lastModifiedBy.SetDevice(nil)
user := msgraphsdk.NewIdentity()
lastModifiedBy.SetUser(user)
id := "366c0b19-49b1-41b5-a03f-9f3887bd0ed8"
user.SetId(&id)
displayName := "John Doe"
user.SetDisplayName(&displayName)
lastModifiedBy.SetAdditionalData(map[string]interface{}{
    "conversation": nil,
}
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
    SetAdditionalData(map[string]interface{}{
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:15:00Z",
        "code": "",
        "displayName": "Lunch",
    }
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
    SetAdditionalData(map[string]interface{}{
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:30:00Z",
        "code": "",
        "displayName": "Lunch",
    }
}
headers := map[string]string{
    "Prefer": "return=representation"
}
options := &msgraphsdk.ShiftRequestBuilderPatchOptions{
    Body: requestBody,
    H: headers,
}
teamId := "team-id"
shiftId := "shift-id"
graphClient.TeamsById(&teamId).Schedule().ShiftsById(&shiftId).Patch(options)


```