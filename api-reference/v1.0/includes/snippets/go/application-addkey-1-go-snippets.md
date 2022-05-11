---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d186d999092578bffa11836eddbb22cf871323d0
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327246"
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
applicationId := "application-id"
result, err := graphClient.ApplicationsById(&applicationId).AddKey(application-id).Post(requestBody)


```