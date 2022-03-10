---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce54f853ad1d675ac26277d8043134d0c6515979
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411799"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTiIndicator()
additionalInformation := "additionalInformation-after-update"
requestBody.SetAdditionalInformation(&additionalInformation)
confidence := int32(42)
requestBody.SetConfidence(&confidence)
description := "description-after-update"
requestBody.SetDescription(&description)
headers := map[string]string{
    "Prefer": "return=representation"
}
options := &msgraphsdk.TiIndicatorRequestBuilderPatchOptions{
    Body: requestBody,
    H: headers,
}
tiIndicatorId := "tiIndicator-id"
result, err := graphClient.Security().TiIndicatorsById(&tiIndicatorId).Patch(options)


```