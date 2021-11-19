---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 34c695452b10f23f01cd77303a6f99f958b5545d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61099610"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
    "draftOpenShift": nil,
}
options := &msgraphsdk.OpenShiftRequestBuilderPutOptions{
    Body: requestBody,
}
teamId := "team-id"
openShiftId := "openShift-id"
graphClient.TeamsById(&teamId).Schedule().OpenShiftsById(&openShiftId).Put(options)


```