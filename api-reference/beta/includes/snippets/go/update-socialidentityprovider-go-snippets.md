---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7dba6057b8286f6843178a01957a308cf8dce9c3
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085384"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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