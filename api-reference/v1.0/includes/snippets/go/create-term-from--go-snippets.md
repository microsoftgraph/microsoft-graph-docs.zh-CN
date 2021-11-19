---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 90ec2d4ed3f7e476c5266a8c33e6064529f666ba
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090512"
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
siteId := "site-id"
setId := "set-id"
result, err := graphClient.SitesById(&siteId).TermStore().SetsById(&setId).Children().Post(options)


```