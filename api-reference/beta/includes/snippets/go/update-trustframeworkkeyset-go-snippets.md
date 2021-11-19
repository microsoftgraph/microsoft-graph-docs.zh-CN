---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e2e74574dc7783999c916f6d8b755930c1daeedc
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084776"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "keys":  []Object {
    }
}
options := &msgraphsdk.TrustFrameworkKeySetRequestBuilderPutOptions{
    Body: requestBody,
}
trustFrameworkKeySetId := "trustFrameworkKeySet-id"
graphClient.TrustFramework().KeySetsById(&trustFrameworkKeySetId).Put(options)


```