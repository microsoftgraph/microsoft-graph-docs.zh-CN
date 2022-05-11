---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8171523dcf3ba74bf84bb69e80b20b220c2b2ce8
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325763"
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
options := &msgraphsdk.TimeOffReasonRequestBuilderPutRequestConfiguration{
    Headers: headers,
}
teamId := "team-id"
timeOffReasonId := "timeOffReason-id"
graphClient.TeamsById(&teamId).Schedule().TimeOffReasonsById(&timeOffReasonId).PutWithRequestConfigurationAndResponseHandler(requestBody, options, nil)


```