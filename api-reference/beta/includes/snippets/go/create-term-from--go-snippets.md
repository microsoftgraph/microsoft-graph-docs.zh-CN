---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1753d2a301a23e8ef48ab820288e1c8028480857
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102271"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTerm()
requestBody.SetLabels( []LocalizedLabel {
    msgraphsdk.NewLocalizedLabel(),
    SetAdditionalData(map[string]interface{}{
        "languageTag": "en-US",
        "name": "Car",
        "isDefault": true,
    }
}
options := &msgraphsdk.ChildrenRequestBuilderPostOptions{
    Body: requestBody,
}
setId := "set-id"
result, err := graphClient.TermStore().SetsById(&setId).Children().Post(options)


```