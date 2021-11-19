---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c3e6d92745c748ac415ba4fc520f1dc5e8b5f974
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082219"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewB2xIdentityUserFlow()
id := "Partner"
requestBody.SetId(&id)
userFlowType := "signUpOrSignIn"
requestBody.SetUserFlowType(&userFlowType)
userFlowTypeVersion := float32(1)
requestBody.SetUserFlowTypeVersion(&userFlowTypeVersion)
options := &msgraphsdk.B2xUserFlowsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Identity().B2xUserFlows().Post(options)


```