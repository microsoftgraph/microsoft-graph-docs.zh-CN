---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bed709ade49a7c0fd9f831521db5c087ff508c8e
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412106"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
keyId := "f0b0b335-1d71-4883-8f98-567911bfdca6"
requestBody.SetKeyId(&keyId)
proof := "eyJ0eXAiOiJ..."
requestBody.SetProof(&proof)
options := &msgraphsdk.RemoveKeyRequestBuilderPostOptions{
    Body: requestBody,
}
servicePrincipalId := "servicePrincipal-id"
graphClient.ServicePrincipalsById(&servicePrincipalId).RemoveKey(servicePrincipal-id).Post(options)


```