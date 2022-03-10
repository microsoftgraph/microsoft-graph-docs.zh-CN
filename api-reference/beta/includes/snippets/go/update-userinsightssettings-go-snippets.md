---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0fb358fd4720d9a7f894a877d3105d76f1c615f4
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412014"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUserInsightsSettings()
isEnabled := "false"
requestBody.SetIsEnabled(&isEnabled)
options := &msgraphsdk.ItemInsightsRequestBuilderPatchOptions{
    Body: requestBody,
}
userId := "user-id"
result, err := graphClient.UsersById(&userId).Settings().ItemInsights().Patch(options)


```