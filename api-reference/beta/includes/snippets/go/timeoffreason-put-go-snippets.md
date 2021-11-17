---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 31e8246fe8449b631dc1d930bfd79a86774593d7
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60977363"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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