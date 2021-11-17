---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 605bdd1dc0dc0bb45bc3aeb52132190fecc17742
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61024176"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewServicePrincipal()
appId := "65415bb1-9267-4313-bbf5-ae259732ee12"
requestBody.SetAppId(&appId)
options := &msgraphsdk.ServicePrincipalsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.ServicePrincipals().Post(options)


```