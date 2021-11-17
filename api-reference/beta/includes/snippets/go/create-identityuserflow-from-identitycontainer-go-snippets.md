---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e4fca041e935318df9803a29cbf61e839fb2150
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61014845"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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