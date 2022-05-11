---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 82c6865c48ff1142cbfea6219bab24fa7e65b492
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327166"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
}
headers := map[string]string{
    "Prefer": "return=representation"
}
options := &msgraphsdk.TimeOffRequestBuilderPutRequestConfiguration{
    Headers: headers,
}
teamId := "team-id"
timeOffId := "timeOff-id"
graphClient.TeamsById(&teamId).Schedule().TimesOffById(&timeOffId).PutWithRequestConfigurationAndResponseHandler(requestBody, options, nil)


```