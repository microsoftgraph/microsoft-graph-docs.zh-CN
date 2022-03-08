---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: daa4e34464fbf010756b27e5848fd278a586f94f
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338317"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAcronym()
displayName := "DNN"
requestBody.SetDisplayName(&displayName)
standsFor := "Deep Neural Network"
requestBody.SetStandsFor(&standsFor)
description := "A deep neural network is a neural network with a certain level of complexity, a neural network with more than two layers."
requestBody.SetDescription(&description)
webUrl := "http://microsoft.com/deep-neural-network"
requestBody.SetWebUrl(&webUrl)
state := "draft"
requestBody.SetState(&state)
options := &msgraphsdk.AcronymsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Search().Acronyms().Post(options)


```