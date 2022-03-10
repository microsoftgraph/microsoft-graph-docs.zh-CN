---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 695a09d16f185dd75a244427f7f9c71b1a52a101
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411706"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
keyCredential := msgraphsdk.NewKeyCredential()
requestBody.SetKeyCredential(keyCredential)
type := "X509CertAndPassword"
keyCredential.SetType(&type)
usage := "Sign"
keyCredential.SetUsage(&usage)
key := []byte("MIIDYDCCAki...")
keyCredential.SetKey(&key)
passwordCredential := msgraphsdk.NewPasswordCredential()
requestBody.SetPasswordCredential(passwordCredential)
secretText := "MKTr0w1..."
passwordCredential.SetSecretText(&secretText)
proof := "eyJ0eXAiOiJ..."
requestBody.SetProof(&proof)
options := &msgraphsdk.AddKeyRequestBuilderPostOptions{
    Body: requestBody,
}
servicePrincipalId := "servicePrincipal-id"
result, err := graphClient.ServicePrincipalsById(&servicePrincipalId).AddKey(servicePrincipal-id).Post(options)


```