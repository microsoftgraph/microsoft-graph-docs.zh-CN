---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a63b248089637cc1a1f12192ee92bf180be282b2
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61031673"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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