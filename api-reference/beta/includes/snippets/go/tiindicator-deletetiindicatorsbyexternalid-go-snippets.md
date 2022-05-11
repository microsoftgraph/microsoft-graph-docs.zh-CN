---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b0cdcef6170510b9d2228794ac7921b2b0d548b
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65329120"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewValueRequestBody()
requestBody.SetValue( []String {
    "externalId-value1",
    "externalId-value2",
}
result, err := graphClient.Security().TiIndicators().DeleteTiIndicatorsByExternalId().Post(requestBody)


```