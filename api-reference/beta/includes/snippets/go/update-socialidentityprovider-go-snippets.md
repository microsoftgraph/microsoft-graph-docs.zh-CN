---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a18d91ae9cf5687c87c314ad25f54ec77f2be94
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61014947"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewIdentityProviderBase()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.socialIdentityProvider",
    "clientSecret": "1111111111111",
}
options := &msgraphsdk.IdentityProviderBaseRequestBuilderPatchOptions{
    Body: requestBody,
}
identityProviderBaseId := "identityProviderBase-id"
graphClient.Identity().IdentityProvidersById(&identityProviderBaseId).Patch(options)


```