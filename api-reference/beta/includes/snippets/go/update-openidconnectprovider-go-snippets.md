---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 254ae8d2249fe670122a91e365cc9ef09d14b5e9
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61014945"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewIdentityProvider()
requestBody.SetAdditionalData(map[string]interface{}{
    "responseType": "id_token",
}
options := &msgraphsdk.IdentityProviderRequestBuilderPatchOptions{
    Body: requestBody,
}
identityProviderId := "identityProvider-id"
graphClient.IdentityProvidersById(&identityProviderId).Patch(options)


```