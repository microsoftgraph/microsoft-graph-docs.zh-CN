---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0589daf5cf499075154fafea02a3b3eed4884dd
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328488"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
    "draftOpenShift": nil,
}
teamId := "team-id"
openShiftId := "openShift-id"
graphClient.TeamsById(&teamId).Schedule().OpenShiftsById(&openShiftId).Put(requestBody)


```