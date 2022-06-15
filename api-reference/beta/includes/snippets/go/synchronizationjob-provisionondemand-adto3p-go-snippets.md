---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 25dee8ac9cef2a4004236b2f5039889d297021bf
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098827"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewParametersRequestBody()
requestBody.SetParameters( []SynchronizationJobApplicationParameters {
    msgraphsdk.NewSynchronizationJobApplicationParameters(),
    SetSubjects( []SynchronizationJobSubject {
        msgraphsdk.NewSynchronizationJobSubject(),
objectId := "9bb0f679-a883-4a6f-8260-35b491b8b8c8"
        SetObjectId(&objectId)
objectTypeName := "User"
        SetObjectTypeName(&objectTypeName)
    }
ruleId := "ea807875-5618-4f0a-9125-0b46a05298ca"
    SetRuleId(&ruleId)
}
servicePrincipalId := "servicePrincipal-id"
synchronizationJobId := "synchronizationJob-id"
result, err := graphClient.ServicePrincipalsById(&servicePrincipalId).Synchronization().JobsById(&synchronizationJobId).ProvisionOnDemand(servicePrincipal-id, synchronizationJob-id).Post(requestBody)


```