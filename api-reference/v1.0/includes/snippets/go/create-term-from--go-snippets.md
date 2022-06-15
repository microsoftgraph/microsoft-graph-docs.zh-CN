---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29eea59ffd756c8bbc3a083faca6eef63f5be2d3
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098818"
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
siteId := "site-id"
setId := "set-id"
result, err := graphClient.SitesById(&siteId).TermStore().SetsById(&setId).Children().Post(requestBody)


```