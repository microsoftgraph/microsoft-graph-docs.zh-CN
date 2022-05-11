---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eab13954a1b3cd373252e1189754f85d04cda492
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65329124"
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
options := &msgraphsdk.RestartRequestBuilderPostRequestConfiguration{
    Headers: headers,
}
servicePrincipalId := "servicePrincipal-id"
synchronizationJobId := "synchronizationJob-id"
graphClient.ServicePrincipalsById(&servicePrincipalId).Synchronization().JobsById(&synchronizationJobId).Restart(servicePrincipal-id, synchronizationJob-id).PostWithRequestConfigurationAndResponseHandler(requestBody, options, nil)


```