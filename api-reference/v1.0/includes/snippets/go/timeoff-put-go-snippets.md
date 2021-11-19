---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06264aa25ce0c6d7aa0baf688d6bfdbf078d4a2e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088164"
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
options := &msgraphsdk.TimeOffRequestBuilderPutOptions{
    Body: requestBody,
    H: headers,
}
teamId := "team-id"
timeOffId := "timeOff-id"
graphClient.TeamsById(&teamId).Schedule().TimesOffById(&timeOffId).Put(options)


```