---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fdc32e18fb57b8b29d9512e28eb9f86199aeb987
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411790"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewIdentityProvider()
clientSecret := "1111111111111"
requestBody.SetClientSecret(&clientSecret)
options := &msgraphsdk.IdentityProviderRequestBuilderPatchOptions{
    Body: requestBody,
}
identityProviderId := "identityProvider-id"
result, err := graphClient.IdentityProvidersById(&identityProviderId).Patch(options)


```