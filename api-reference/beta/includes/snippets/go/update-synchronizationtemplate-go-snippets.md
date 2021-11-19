---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 34bcddef77072e8fcaf5237543372b0850266985
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092699"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "id": "Slack",
    "applicationId": "{id}",
    "factoryTag": "CustomSCIM",
}
headers := map[string]string{
    "Authorization": "Bearer <token>"
}
options := &msgraphsdk.SynchronizationTemplateRequestBuilderPutOptions{
    Body: requestBody,
    H: headers,
}
applicationId := "application-id"
synchronizationTemplateId := "synchronizationTemplate-id"
graphClient.ApplicationsById(&applicationId).Synchronization().TemplatesById(&synchronizationTemplateId).Put(options)


```