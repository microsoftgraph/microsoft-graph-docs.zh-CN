---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c4a890d0c49480397eae4e03235755df9249574f
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65719298"
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
    SetAdditionalData(map[string]interface{}{
        "languageTag": "es-es",
        "displayName": "Sitio de instalación Contoso",
        "description": "Pruebe o compre Contoso hogar o negocios y vea la información del producto",
    }
}
state := "published"
requestBody.SetState(&state)
result, err := graphClient.Search().Bookmarks().Post(requestBody)


```