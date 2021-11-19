---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: daa16fcb00779b02a957dc97c504073ca5584f02
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61099149"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOpenShift()
schedulingGroupId := "TAG_228940ed-ff84-4e25-b129-1b395cf78be0"
requestBody.SetSchedulingGroupId(&schedulingGroupId)
sharedOpenShift := msgraphsdk.NewOpenShiftItem()
requestBody.SetSharedOpenShift(sharedOpenShift)
sharedOpenShift.SetAdditionalData(map[string]interface{}{
    "notes": "Inventory Management",
    "openSlotCount": ,
    "displayName": "Field shift",
    "startDateTime": "2018-10-04T00:58:45.340Z",
    "endDateTime": "2018-10-04T09:50:45.332Z",
    "theme": "white",
    "activities":  []Object {
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