---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 79b074893bf5f30db3ba77d9cd5aef099266108c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61033655"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "enabled": true,
    "timeZone": "America/Chicago",
    "provisionStatus": "Completed",
    "provisionStatusCode": nil,
    "openShiftsEnabled": true,
    "swapShiftsRequestsEnabled": true,
    "offerShiftRequestsEnabled": true,
    "timeOffRequestsEnabled": true,
    "timeClockEnabled": true,
}
options := &msgraphsdk.ScheduleRequestBuilderPutOptions{
    Body: requestBody,
}
teamId := "team-id"
graphClient.TeamsById(&teamId).Schedule().Put(options)


```