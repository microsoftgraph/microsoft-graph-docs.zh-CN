---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 791210f47a869a2a99dfb7f4039e194cc5d2e47f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328837"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAcronym()
description := "A deep neural network is a neural network with a certain level of complexity, a neural network with more than two layers."
requestBody.SetDescription(&description)
acronymId := "acronym-id"
graphClient.Search().AcronymsById(&acronymId).Patch(requestBody)


```