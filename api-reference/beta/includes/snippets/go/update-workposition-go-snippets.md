---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 335da60dd681b6be89ba26755f02768c557d5d78
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412739"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewWorkPosition()
isCurrent := true
requestBody.SetIsCurrent(&isCurrent)
options := &msgraphsdk.WorkPositionRequestBuilderPatchOptions{
    Body: requestBody,
}
workPositionId := "workPosition-id"
result, err := graphClient.Me().Profile().PositionsById(&workPositionId).Patch(options)


```