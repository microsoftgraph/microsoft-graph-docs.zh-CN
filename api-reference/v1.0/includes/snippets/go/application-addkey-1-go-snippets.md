---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 25381c295395a5cda28d2b82e8e628e2f7d31d54
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085934"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
keyCredential := msgraphsdk.NewKeyCredential()
requestBody.SetKeyCredential(keyCredential)
type := "AsymmetricX509Cert"
keyCredential.SetType(&type)
usage := "Verify"
keyCredential.SetUsage(&usage)
key := []byte("MIIDYDCCAki...")
keyCredential.SetKey(&key)
requestBody.SetPasswordCredential(nil)
proof := "eyJ0eXAiOiJ..."
requestBody.SetProof(&proof)
options := &msgraphsdk.AddKeyRequestBuilderPostOptions{
    Body: requestBody,
}
applicationId := "application-id"
result, err := graphClient.ApplicationsById(&applicationId).AddKey().Post(options)


```