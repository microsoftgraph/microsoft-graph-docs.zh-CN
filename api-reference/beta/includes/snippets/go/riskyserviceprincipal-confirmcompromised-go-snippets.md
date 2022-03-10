---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 42bb65a3ef342f8dc4ac157ff1bc691d1f0f84f9
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412495"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewServicePrincipalIdsRequestBody()
requestBody.SetServicePrincipalIds( []String {
    "9089a539-a539-9089-39a5-899039a58990",
}
options := &msgraphsdk.ConfirmCompromisedRequestBuilderPostOptions{
    Body: requestBody,
}
graphClient.IdentityProtection().RiskyServicePrincipals().ConfirmCompromised().Post(options)


```