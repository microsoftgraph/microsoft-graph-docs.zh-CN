---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d180a3606a77604d0e26468f44cda118fa25fcf
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326959"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "displayName": "Cashiers",
    "isActive": true,
    "userIds":  []String {
        "c5d0c76b-80c4-481c-be50-923cd8d680a1",
        "2a4296b3-a28a-44ba-bc66-0274b9b95851",
    }
}
headers := map[string]string{
    "Prefer": "return=representation"
}
options := &msgraphsdk.SchedulingGroupRequestBuilderPutRequestConfiguration{
    Headers: headers,
}
teamId := "team-id"
schedulingGroupId := "schedulingGroup-id"
graphClient.TeamsById(&teamId).Schedule().SchedulingGroupsById(&schedulingGroupId).PutWithRequestConfigurationAndResponseHandler(requestBody, options, nil)


```