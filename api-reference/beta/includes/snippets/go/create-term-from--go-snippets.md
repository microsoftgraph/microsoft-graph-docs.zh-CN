---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 65162c31ef3c3bafe8c660ac981c916fbe93ab5b
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094839"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTerm()
requestBody.SetLabels( []LocalizedLabel {
    msgraphsdk.NewLocalizedLabel(),
languageTag := "en-US"
    SetLanguageTag(&languageTag)
name := "Car"
    SetName(&name)
isDefault := true
    SetIsDefault(&isDefault)
}
setId := "set-id"
result, err := graphClient.TermStore().SetsById(&setId).Children().Post(requestBody)


```