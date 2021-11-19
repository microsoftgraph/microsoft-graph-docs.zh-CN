---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d50038885e83aeee9cc7c03fcc1be49511b734cf
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090669"
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
graphClient.Identity().ConditionalAccess().AuthenticationContextClassReferencesById(&authenticationContextClassReferenceId).Patch(options)


```