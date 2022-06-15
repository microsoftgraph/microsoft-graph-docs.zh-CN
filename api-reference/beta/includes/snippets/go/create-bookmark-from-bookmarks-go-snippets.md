---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 133d933142a89a70958aa94aa5aaa17e397eea29
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098675"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewBookmark()
displayName := "Contoso Install Site"
requestBody.SetDisplayName(&displayName)
webUrl := "http://www.contoso.com/"
requestBody.SetWebUrl(&webUrl)
description := "Try or buy Contoso for Home or Business and view product information"
requestBody.SetDescription(&description)
keywords := msgraphsdk.NewAnswerKeyword()
requestBody.SetKeywords(keywords)
keywords.SetKeywords( []String {
    "Contoso",
    "install",
}
keywords.SetReservedKeywords( []String {
    "Contoso",
}
matchSimilarKeywords := true
keywords.SetMatchSimilarKeywords(&matchSimilarKeywords)
requestBody.SetAvailabilityStartDateTime(nil)
requestBody.SetAvailabilityEndDateTime(nil)
requestBody.SetPlatforms( []DevicePlatformType {
    "windows",
}
requestBody.SetTargetedVariations( []AnswerVariant {
    msgraphsdk.NewAnswerVariant(),
languageTag := "es-es"
    SetLanguageTag(&languageTag)
displayName := "Sitio de instalación Contoso"
    SetDisplayName(&displayName)
description := "Pruebe o compre Contoso hogar o negocios y vea la información del producto"
    SetDescription(&description)
}
state := "published"
requestBody.SetState(&state)
result, err := graphClient.Search().Bookmarks().Post(requestBody)


```