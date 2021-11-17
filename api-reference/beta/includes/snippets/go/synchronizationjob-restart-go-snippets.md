---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6356199bcf8e6ea5664b7af243adacedee5bd561
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61033711"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
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
graphClient.ServicePrincipalsById(&servicePrincipalId).Synchronization().JobsById(&synchronizationJobId).Restart().Post(options)


```