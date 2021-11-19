---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 27b76a80fdb94160d34cee665325866b9423f817
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084833"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewServicePrincipal()
appId := "65415bb1-9267-4313-bbf5-ae259732ee12"
requestBody.SetAppId(&appId)
options := &msgraphsdk.ServicePrincipalsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.ServicePrincipals().Post(options)


```