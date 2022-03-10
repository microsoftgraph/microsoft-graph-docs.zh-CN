---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f7d0529f2ae78cf6ad6e57d0bb641f30419b26b7
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411661"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewGroup()
description := "Contoso Life v2.0"
requestBody.SetDescription(&description)
displayName := "Contoso Life Renewed"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.GroupRequestBuilderPatchOptions{
    Body: requestBody,
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).Patch(options)


```