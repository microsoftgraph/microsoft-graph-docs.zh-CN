---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 836461f339c303697570021338f04b9c1dbd09a5
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412581"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAcronym()
description := "A deep neural network is a neural network with a certain level of complexity, a neural network with more than two layers."
requestBody.SetDescription(&description)
options := &msgraphsdk.AcronymRequestBuilderPatchOptions{
    Body: requestBody,
}
acronymId := "acronym-id"
result, err := graphClient.Search().AcronymsById(&acronymId).Patch(options)


```