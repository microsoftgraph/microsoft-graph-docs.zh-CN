---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e844cfba0ee117e4039aa66597d5764c49a2e635
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412246"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewItemEmail()
displayName := "Business Email"
requestBody.SetDisplayName(&displayName)
type := "work"
requestBody.SetType(&type)
options := &msgraphsdk.ItemEmailRequestBuilderPatchOptions{
    Body: requestBody,
}
userId := "user-id"
itemEmailId := "itemEmail-id"
result, err := graphClient.UsersById(&userId).Profile().EmailsById(&itemEmailId).Patch(options)


```