---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 56921661a4f91f69a4d066c1898c340b801ef4d8
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61081671"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewGroup()
description := "Group with designated owner and members"
requestBody.SetDescription(&description)
displayName := "Operations group"
requestBody.SetDisplayName(&displayName)
requestBody.SetGroupTypes( []string {
}
mailEnabled := false
requestBody.SetMailEnabled(&mailEnabled)
mailNickname := "operations2019"
requestBody.SetMailNickname(&mailNickname)
securityEnabled := true
requestBody.SetSecurityEnabled(&securityEnabled)
requestBody.SetAdditionalData(map[string]interface{}{
    "owners@odata.bind":  []String {
        "https://graph.microsoft.com/v1.0/users/26be1845-4119-4801-a799-aea79d09f1a2",
    }
    "members@odata.bind":  []String {
        "https://graph.microsoft.com/v1.0/users/ff7cb387-6688-423c-8188-3da9532a73cc",
        "https://graph.microsoft.com/v1.0/users/69456242-0067-49d3-ba96-9de6f2728e14",
    }
}
options := &msgraphsdk.GroupsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Groups().Post(options)


```