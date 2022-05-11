---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 209b3d0f3771e5dd814d8f5f3626ad7f008861c4
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327236"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewGroup()
description := "Self help community for library"
requestBody.SetDescription(&description)
displayName := "Library Assist"
requestBody.SetDisplayName(&displayName)
requestBody.SetGroupTypes( []String {
    "Unified",
}
mailEnabled := true
requestBody.SetMailEnabled(&mailEnabled)
mailNickname := "library"
requestBody.SetMailNickname(&mailNickname)
securityEnabled := false
requestBody.SetSecurityEnabled(&securityEnabled)
result, err := graphClient.Groups().Post(requestBody)


```