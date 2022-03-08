---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0089a377f873b3dc6399022943e83d4624c051a2
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334735"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetServicePrincipalIds( []String {
    "9089a539-a539-9089-39a5-899039a58990",
}
options := &msgraphsdk.ConfirmCompromisedRequestBuilderPostOptions{
    Body: requestBody,
}
graphClient.IdentityProtection().RiskyServicePrincipals().ConfirmCompromised().Post(options)


```