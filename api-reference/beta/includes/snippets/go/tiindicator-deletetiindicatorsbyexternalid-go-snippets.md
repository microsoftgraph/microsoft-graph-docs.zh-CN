---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 00dfea61faf79ab3838059084833915cd1878024
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412024"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewValueRequestBody()
requestBody.SetValue( []String {
    "externalId-value1",
    "externalId-value2",
}
options := &msgraphsdk.DeleteTiIndicatorsByExternalIdRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Security().TiIndicators().DeleteTiIndicatorsByExternalId().Post(options)


```