---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20261716516e01ff52f017344336ccdb94496573
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411742"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewServicePrincipalIdsRequestBody()
requestBody.SetServicePrincipalIds( []String {
    "9089a539-a539-9089-39a5-899039a58990",
}
options := &msgraphsdk.DismissRequestBuilderPostOptions{
    Body: requestBody,
}
graphClient.IdentityProtection().RiskyServicePrincipals().Dismiss().Post(options)


```