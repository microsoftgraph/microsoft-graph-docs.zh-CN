---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2cd58eb64348c83235f6160beb4d09de1527614e
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098828"
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
isPaid := true
    SetIsPaid(&isPaid)
startDateTime, err := time.Parse(time.RFC3339, "2018-10-04T00:58:45.340Z")
    SetStartDateTime(&startDateTime)
endDateTime, err := time.Parse(time.RFC3339, "2018-10-04T01:58:45.340Z")
    SetEndDateTime(&endDateTime)
code := ""
    SetCode(&code)
displayName := "Lunch"
    SetDisplayName(&displayName)
}
requestBody.SetDraftOpenShift(nil)
teamId := "team-id"
openShiftId := "openShift-id"
graphClient.TeamsById(&teamId).Schedule().OpenShiftsById(&openShiftId).Patch(requestBody)


```