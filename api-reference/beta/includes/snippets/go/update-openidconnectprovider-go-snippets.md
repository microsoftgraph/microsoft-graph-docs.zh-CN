---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e78f37688c0038ae92ea71b73d1ad7d2ba98f159
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629797"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewIdentityProvider()
requestBody.SetAdditionalData(map[string]interface{}{
    "responseType": "id_token",
}
identityProviderId := "identityProvider-id"
graphClient.IdentityProvidersById(&identityProviderId).Patch(requestBody)


```