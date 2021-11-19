---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a27bf227be484b6b01ea9cb5895cb29ea2c0f0a
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102591"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewSynchronizationJob()
templateId := "BoxOutDelta"
requestBody.SetTemplateId(&templateId)
options := &msgraphsdk.JobsRequestBuilderPostOptions{
    Body: requestBody,
}
servicePrincipalId := "servicePrincipal-id"
result, err := graphClient.ServicePrincipalsById(&servicePrincipalId).Synchronization().Jobs().Post(options)


```