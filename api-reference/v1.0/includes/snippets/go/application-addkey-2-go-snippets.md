---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5fbf6f30e3c3c3fc6504937b3f71a3344ed106ba
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61029768"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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