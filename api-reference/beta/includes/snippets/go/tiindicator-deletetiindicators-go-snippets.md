---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b7ff7f3d6f5434b6660d008b163d8e7f31ffd415
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412578"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewValueRequestBody()
requestBody.SetValue( []String {
    "id-value1",
    "id-value2",
}
options := &msgraphsdk.DeleteTiIndicatorsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Security().TiIndicators().DeleteTiIndicators().Post(options)


```