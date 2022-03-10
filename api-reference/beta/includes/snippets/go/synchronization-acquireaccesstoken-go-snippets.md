---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8bb80a8eddf1dae7c59bf0c3d92bcbb7b8a5ac3f
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412747"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCredentialsRequestBody()
requestBody.SetCredentials( []SynchronizationSecretKeyStringValuePair {
    msgraphsdk.NewSynchronizationSecretKeyStringValuePair(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "microsoft.graph.synchronizationSecretKeyStringValuePair",
    }
}
options := &msgraphsdk.AcquireAccessTokenRequestBuilderPostOptions{
    Body: requestBody,
}
applicationId := "application-id"
graphClient.ApplicationsById(&applicationId).Synchronization().AcquireAccessToken(application-id).Post(options)


```