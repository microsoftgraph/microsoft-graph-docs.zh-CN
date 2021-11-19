---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b5df56c0c7ecf7ba741cade4f443d77370d6618
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098429"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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