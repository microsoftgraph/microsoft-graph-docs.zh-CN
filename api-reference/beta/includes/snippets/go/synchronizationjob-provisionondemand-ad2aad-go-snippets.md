---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cecca3f34a3b0b245870d075ac47b3937b4c46aa
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202872"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewParametersRequestBody()
requestBody.SetParameters( []SynchronizationJobApplicationParameters {
    msgraphsdk.NewSynchronizationJobApplicationParameters(),
    SetAdditionalData(map[string]interface{}{
        "ruleId": "6c409270-f78a-4bc6-af23-7cf3ab6482fe",
        "subjects":  []Object {
        }
    }
}
options := &msgraphsdk.ProvisionOnDemandRequestBuilderPostOptions{
    Body: requestBody,
}
servicePrincipalId := "servicePrincipal-id"
synchronizationJobId := "synchronizationJob-id"
result, err := graphClient.ServicePrincipalsById(&servicePrincipalId).Synchronization().JobsById(&synchronizationJobId).ProvisionOnDemand(servicePrincipal-id, synchronizationJob-id).Post(options)


```