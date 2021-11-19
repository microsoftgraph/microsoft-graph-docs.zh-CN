---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7005df441bd20fb83a84e51d9d981eb047b6bc7c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084993"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewSynchronizationTemplate()
id := "SCIM-Test1"
requestBody.SetId(&id)
applicationId := "{id}"
requestBody.SetApplicationId(&applicationId)
factoryTag := "CustomSCIM"
requestBody.SetFactoryTag(&factoryTag)
options := &msgraphsdk.TemplatesRequestBuilderPostOptions{
    Body: requestBody,
}
applicationId := "application-id"
result, err := graphClient.ApplicationsById(&applicationId).Synchronization().Templates().Post(options)


```