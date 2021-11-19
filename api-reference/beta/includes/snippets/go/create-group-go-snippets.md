---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b9437863c8b21bb93972a1b45d958f6b441d5d3
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61093791"
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
options := &msgraphsdk.GroupsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Groups().Post(options)


```