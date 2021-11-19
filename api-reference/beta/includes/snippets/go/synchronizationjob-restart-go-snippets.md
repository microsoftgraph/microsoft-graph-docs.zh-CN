---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5aeb019f31ae2d7e09792bb18c0300e83e66da6b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097146"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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