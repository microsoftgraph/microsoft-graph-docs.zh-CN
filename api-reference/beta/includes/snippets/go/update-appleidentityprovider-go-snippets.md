---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a97e9790829cffe7841787fed766aa68f6a6773d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085587"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewIdentityProviderBase()
displayName := "Apple"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.IdentityProviderBaseRequestBuilderPatchOptions{
    Body: requestBody,
}
identityProviderBaseId := "identityProviderBase-id"
graphClient.Identity().IdentityProvidersById(&identityProviderBaseId).Patch(options)


```