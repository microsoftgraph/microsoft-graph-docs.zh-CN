---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 26132df72e753d415b123b5e540b50f593aab2fd
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338241"
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
        "languageTag": "es-ES",
        "displayName": "Sitio de instalación Contoso",
        "description": "Pruebe o compre Contoso hogar o negocios y vea la información del producto",
    }
}
requestBody.SetGroupIds( []String {
    "groupId",
}
requestBody.SetPowerAppIds( []String {
    "powerAppId",
}
state := "published"
requestBody.SetState(&state)
options := &msgraphsdk.BookmarksRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Search().Bookmarks().Post(options)


```