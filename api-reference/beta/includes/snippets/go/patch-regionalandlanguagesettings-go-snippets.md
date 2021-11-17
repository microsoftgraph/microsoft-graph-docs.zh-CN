---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: debc398810b30e4555ca747aa7311a7bb3f2653c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60996884"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewRegionalAndLanguageSettings()
requestBody.SetAuthoringLanguages( []LocaleInfo {
    msgraphsdk.NewLocaleInfo(),
    SetAdditionalData(map[string]interface{}{
        "locale": "en-US",
    }
    msgraphsdk.NewLocaleInfo(),
    SetAdditionalData(map[string]interface{}{
        "locale": "es-MX",
    }
}
defaultRegionalFormat := msgraphsdk.NewLocaleInfo()
requestBody.SetDefaultRegionalFormat(defaultRegionalFormat)
locale := "en-US"
defaultRegionalFormat.SetLocale(&locale)
options := &msgraphsdk.RegionalAndLanguageSettingsRequestBuilderPatchOptions{
    Body: requestBody,
}
graphClient.Me().Settings().RegionalAndLanguageSettings().Patch(options)


```