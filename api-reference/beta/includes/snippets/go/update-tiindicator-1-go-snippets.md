---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ab8a2b00444b29f62f00a37392efa699417656e
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411798"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTiIndicator()
description := "description-updated"
requestBody.SetDescription(&description)
options := &msgraphsdk.TiIndicatorRequestBuilderPatchOptions{
    Body: requestBody,
}
tiIndicatorId := "tiIndicator-id"
result, err := graphClient.Security().TiIndicatorsById(&tiIndicatorId).Patch(options)


```