---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 02d98bcadd08fd59b53764de652b866f21cb0c76
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61001642"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
requestBody.SetValue( []String {
    "id-value1",
    "id-value2",
}
options := &msgraphsdk.DeleteTiIndicatorsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Security().TiIndicators().DeleteTiIndicators().Post(options)


```