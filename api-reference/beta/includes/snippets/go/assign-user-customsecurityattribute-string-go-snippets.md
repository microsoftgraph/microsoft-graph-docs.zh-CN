---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9dd0fcef38ad758301fef1d774c437aed37f2ac2
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412018"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUser()
customSecurityAttributes := msgraphsdk.NewCustomSecurityAttributeValue()
requestBody.SetCustomSecurityAttributes(customSecurityAttributes)
customSecurityAttributes.SetAdditionalData(map[string]interface{}{
}
options := &msgraphsdk.UserRequestBuilderPatchOptions{
    Body: requestBody,
}
userId := "user-id"
result, err := graphClient.UsersById(&userId).Patch(options)


```