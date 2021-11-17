---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 386f17f76f906d8622d39180dfacce8e07a1a1a0
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60990778"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/identity/identityProviders/B2X_1_Test",
    "@odata.type": "#microsoft.graph.identityProvider",
}
options := &msgraphsdk.RefRequestBuilderPatchOptions{
    Body: requestBody,
}
b2xIdentityUserFlowId := "b2xIdentityUserFlow-id"
graphClient.Identity().B2xUserFlowsById(&b2xIdentityUserFlowId).UserFlowIdentityProviders().$ref().Patch(options)


```