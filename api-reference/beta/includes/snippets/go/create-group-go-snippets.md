---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c37c61837682b6e7b85107e3a07cee42d35e8d1a
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65329236"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewGroup()
description := "Self help community for golf"
requestBody.SetDescription(&description)
displayName := "Golf Assist"
requestBody.SetDisplayName(&displayName)
requestBody.SetGroupTypes( []String {
    "Unified",
}
mailEnabled := true
requestBody.SetMailEnabled(&mailEnabled)
mailNickname := "golfassist"
requestBody.SetMailNickname(&mailNickname)
securityEnabled := false
requestBody.SetSecurityEnabled(&securityEnabled)
result, err := graphClient.Groups().Post(requestBody)


```