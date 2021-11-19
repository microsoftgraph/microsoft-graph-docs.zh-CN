---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cbfcf3dff911d80f8e1c9dac66e0353af4600d8c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086750"
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
applicationId := "application-id"
result, err := graphClient.ApplicationsById(&applicationId).AddKey().Post(options)


```