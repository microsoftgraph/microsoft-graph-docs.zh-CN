---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a17f66c0b5710f29f0b7e0a58cf07fe8978c9b6b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089459"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewIdentityUserFlow()
id := "Pol1"
requestBody.SetId(&id)
userFlowType := "signUpOrSignIn"
requestBody.SetUserFlowType(&userFlowType)
userFlowTypeVersion := float32(1)
requestBody.SetUserFlowTypeVersion(&userFlowTypeVersion)
options := &msgraphsdk.UserFlowsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Identity().UserFlows().Post(options)


```