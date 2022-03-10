---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 52cda61456831d234a2e53a881b9c91a6b7d8da5
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412183"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAuthenticationContextClassReference()
requestBody.SetAdditionalData(map[string]interface{}{
    "value":  []Object {
    }
}
options := &msgraphsdk.AuthenticationContextClassReferenceRequestBuilderPatchOptions{
    Body: requestBody,
}
authenticationContextClassReferenceId := "authenticationContextClassReference-id"
result, err := graphClient.Identity().ConditionalAccess().AuthenticationContextClassReferencesById(&authenticationContextClassReferenceId).Patch(options)


```