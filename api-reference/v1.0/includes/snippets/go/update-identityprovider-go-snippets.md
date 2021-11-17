---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 74d4dc4638b4486cffd0cff28835d06b01e37acc
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61024505"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewIdentityProvider()
clientSecret := "1111111111111"
requestBody.SetClientSecret(&clientSecret)
options := &msgraphsdk.IdentityProviderRequestBuilderPatchOptions{
    Body: requestBody,
}
identityProviderId := "identityProvider-id"
graphClient.IdentityProvidersById(&identityProviderId).Patch(options)


```