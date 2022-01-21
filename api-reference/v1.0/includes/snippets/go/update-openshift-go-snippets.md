---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 196c9d3815140e48565b03636b89e9c5bbde4f97
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62128602"
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
graphClient.TeamsById(&teamId).Schedule().OpenShiftsById(&openShiftId).Patch(options)


```