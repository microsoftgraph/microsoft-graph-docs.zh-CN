---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 31e705d4b0d04159b7ddaca41f4924488bedbe17
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326333"
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
groupId := "group-id"
graphClient.GroupsById(&groupId).Patch(requestBody)


```