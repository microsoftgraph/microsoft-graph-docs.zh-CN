---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c3d5291bfe0ad5e5c7b1773af7c00d04bd2d4aa
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326449"
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
result, err := graphClient.Search().Acronyms().Post(requestBody)


```