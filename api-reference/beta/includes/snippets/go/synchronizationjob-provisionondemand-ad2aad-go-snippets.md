---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 17c1cc350c7e731f9a02314ad10f2e9ea85734ff
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098826"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewParametersRequestBody()
requestBody.SetParameters( []SynchronizationJobApplicationParameters {
    msgraphsdk.NewSynchronizationJobApplicationParameters(),
ruleId := "6c409270-f78a-4bc6-af23-7cf3ab6482fe"
    SetRuleId(&ruleId)
    SetSubjects( []SynchronizationJobSubject {
        msgraphsdk.NewSynchronizationJobSubject(),
objectId := "CN=AdeleV,CN=Users,DC=corp,DC=chicago,DC=com"
        SetObjectId(&objectId)
objectTypeName := "user"
        SetObjectTypeName(&objectTypeName)
    }
}
servicePrincipalId := "servicePrincipal-id"
synchronizationJobId := "synchronizationJob-id"
result, err := graphClient.ServicePrincipalsById(&servicePrincipalId).Synchronization().JobsById(&synchronizationJobId).ProvisionOnDemand(servicePrincipal-id, synchronizationJob-id).Post(requestBody)


```