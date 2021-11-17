---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16f07ca6f5a13cd4a528bcf85e4aafc58508a288
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61001593"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
}
headers := map[string]string{
    "Prefer": "return=representation"
}
options := &msgraphsdk.TimeOffRequestBuilderPutOptions{
    Body: requestBody,
    H: headers,
}
teamId := "team-id"
timeOffId := "timeOff-id"
graphClient.TeamsById(&teamId).Schedule().TimesOffById(&timeOffId).Put(options)


```