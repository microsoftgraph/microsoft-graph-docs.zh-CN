---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c8a33617612e54eb49995e62007650fff525cdba
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411704"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
displayName := "CN=customDisplayName"
requestBody.SetDisplayName(&displayName)
endDateTime, err := time.Parse(time.RFC3339, "2024-01-25T00:00:00Z")
requestBody.SetEndDateTime(&endDateTime)
options := &msgraphsdk.AddTokenSigningCertificateRequestBuilderPostOptions{
    Body: requestBody,
}
servicePrincipalId := "servicePrincipal-id"
result, err := graphClient.ServicePrincipalsById(&servicePrincipalId).AddTokenSigningCertificate(servicePrincipal-id).Post(options)


```