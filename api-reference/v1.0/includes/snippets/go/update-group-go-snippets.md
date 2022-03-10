---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1432b265fbc7a7ffe699542c3eb057428648f2d3
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412000"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewGroup()
description := "Library Assist"
requestBody.SetDescription(&description)
displayName := "Library Assist"
requestBody.SetDisplayName(&displayName)
requestBody.SetGroupTypes( []String {
    "Unified",
}
mailEnabled := true
requestBody.SetMailEnabled(&mailEnabled)
mailNickname := "library-help"
requestBody.SetMailNickname(&mailNickname)
options := &msgraphsdk.GroupRequestBuilderPatchOptions{
    Body: requestBody,
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).Patch(options)


```