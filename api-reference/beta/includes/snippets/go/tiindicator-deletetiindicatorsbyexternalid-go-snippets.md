---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d975474b13d2f84e74c245997f30ff000af5117c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60977419"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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