---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 26420a4b7a15f9ee13dd177c19c6f025ef1a613d
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412113"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOpenShift()
schedulingGroupId := "TAG_228940ed-ff84-4e25-b129-1b395cf78be0"
requestBody.SetSchedulingGroupId(&schedulingGroupId)
sharedOpenShift := msgraphsdk.NewOpenShiftItem()
requestBody.SetSharedOpenShift(sharedOpenShift)
notes := "Inventory Management"
sharedOpenShift.SetNotes(&notes)
openSlotCount := int32(5)
sharedOpenShift.SetOpenSlotCount(&openSlotCount)
displayName := "Field shift"
sharedOpenShift.SetDisplayName(&displayName)
startDateTime, err := time.Parse(time.RFC3339, "2018-10-04T00:58:45.340Z")
sharedOpenShift.SetStartDateTime(&startDateTime)
endDateTime, err := time.Parse(time.RFC3339, "2018-10-04T09:50:45.332Z")
sharedOpenShift.SetEndDateTime(&endDateTime)
theme := "white"
sharedOpenShift.SetTheme(&theme)
sharedOpenShift.SetActivities( []ShiftActivity {
    msgraphsdk.NewShiftActivity(),
    SetAdditionalData(map[string]interface{}{
        "isPaid": true,
        "startDateTime": "2018-10-04T00:58:45.340Z",
        "endDateTime": "2018-10-04T01:58:45.340Z",
        "code": "",
        "displayName": "Lunch",
    }
}
requestBody.SetDraftOpenShift(nil)
options := &msgraphsdk.OpenShiftRequestBuilderPatchOptions{
    Body: requestBody,
}
teamId := "team-id"
openShiftId := "openShift-id"
result, err := graphClient.TeamsById(&teamId).Schedule().OpenShiftsById(&openShiftId).Patch(options)


```