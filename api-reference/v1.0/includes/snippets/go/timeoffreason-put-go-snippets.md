---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57d7e5f22a5535ddba3ef04483739789a3bf58bb
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098723"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "displayName": "Vacation",
    "iconType": "plane",
    "isActive": true,
}
headers := map[string]string{
    "Prefer": "return=representation"
}
options := &msgraphsdk.TimeOffReasonRequestBuilderPutOptions{
    Body: requestBody,
    H: headers,
}
teamId := "team-id"
timeOffReasonId := "timeOffReason-id"
graphClient.TeamsById(&teamId).Schedule().TimeOffReasonsById(&timeOffReasonId).Put(options)


```