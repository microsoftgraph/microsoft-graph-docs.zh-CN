---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fbbf87da0b37f39da1a840332b8545da29034007
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412347"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCriteriaRequestBody()
criteria := msgraphsdk.NewSynchronizationJobRestartCriteria()
requestBody.SetCriteria(criteria)
resetScope := "Watermark, Escrows, QuarantineState"
criteria.SetResetScope(&resetScope)
headers := map[string]string{
    "Authorization": "Bearer <token>"
}
options := &msgraphsdk.RestartRequestBuilderPostOptions{
    Body: requestBody,
    H: headers,
}
servicePrincipalId := "servicePrincipal-id"
synchronizationJobId := "synchronizationJob-id"
graphClient.ServicePrincipalsById(&servicePrincipalId).Synchronization().JobsById(&synchronizationJobId).Restart(servicePrincipal-id, synchronizationJob-id).Post(options)


```