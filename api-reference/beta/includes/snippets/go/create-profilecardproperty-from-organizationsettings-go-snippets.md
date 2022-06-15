---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b977d171596030f2cba97bc23a5fac2dfa447ce3
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098816"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewProfileCardProperty()
directoryPropertyName := "CustomAttribute1"
requestBody.SetDirectoryPropertyName(&directoryPropertyName)
requestBody.SetAnnotations( []ProfileCardAnnotation {
    msgraphsdk.NewProfileCardAnnotation(),
displayName := "Cost Center"
    SetDisplayName(&displayName)
    SetLocalizations( []DisplayNameLocalization {
        msgraphsdk.NewDisplayNameLocalization(),
languageTag := "ru-RU"
        SetLanguageTag(&languageTag)
displayName := "центр затрат"
        SetDisplayName(&displayName)
    }
}
organizationId := "organization-id"
result, err := graphClient.OrganizationById(&organizationId).Settings().ProfileCardProperties().Post(requestBody)


```