---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f2fb5074a268a276a7e629a70d61d4133dc74dac
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087982"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
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
graphClient.ApplicationsById(&applicationId).Synchronization().AcquireAccessToken().Post(options)


```