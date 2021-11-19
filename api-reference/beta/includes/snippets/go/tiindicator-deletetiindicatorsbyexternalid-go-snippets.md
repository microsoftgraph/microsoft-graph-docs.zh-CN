---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e432a6ccd44acaebaa06806d7f64dae36c56247c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097257"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetValue( []String {
    "externalId-value1",
    "externalId-value2",
}
options := &msgraphsdk.DeleteTiIndicatorsByExternalIdRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Security().TiIndicators().DeleteTiIndicatorsByExternalId().Post(options)


```