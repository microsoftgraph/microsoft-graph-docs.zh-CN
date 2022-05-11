---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 55838ac530379ad75e381a5a8e5468c887975c8f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327763"
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
servicePrincipalId := "servicePrincipal-id"
result, err := graphClient.ServicePrincipalsById(&servicePrincipalId).AddKey(servicePrincipal-id).Post(requestBody)


```