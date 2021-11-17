---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3538ccf1ca06ad6631407624ba7da4b877b41e77
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60977797"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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