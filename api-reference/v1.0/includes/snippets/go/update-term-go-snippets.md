---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 86905c9e38c32221de27a3f570c8d89197877883
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412103"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTerm()
requestBody.SetLabels( []LocalizedLabel {
    msgraphsdk.NewLocalizedLabel(),
    SetAdditionalData(map[string]interface{}{
        "name": "changedLabel",
        "languageTag": "en-US",
        "isDefault": true,
    }
}
options := &msgraphsdk.TermRequestBuilderPatchOptions{
    Body: requestBody,
}
siteId := "site-id"
setId := "set-id"
termId := "term-id"
result, err := graphClient.SitesById(&siteId).TermStore().SetsById(&setId).TermsById(&termId).Patch(options)


```