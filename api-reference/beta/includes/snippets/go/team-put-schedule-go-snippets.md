---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4525479d0d6ef5eccfa9879987ecad6c93930e80
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61033656"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "enabled": true,
    "timeZone": "America/Chicago",
}
options := &msgraphsdk.ScheduleRequestBuilderPutOptions{
    Body: requestBody,
}
teamId := "team-id"
graphClient.TeamsById(&teamId).Schedule().Put(options)


```