---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7dd084f7e2ee2e9be1c0eb35b7761bb36069a1be
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098709"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTerm()
requestBody.SetLabels( []LocalizedLabel {
    msgraphsdk.NewLocalizedLabel(),
name := "changedLabel"
    SetName(&name)
languageTag := "en-US"
    SetLanguageTag(&languageTag)
isDefault := true
    SetIsDefault(&isDefault)
}
siteId := "site-id"
setId := "set-id"
termId := "term-id"
graphClient.SitesById(&siteId).TermStore().SetsById(&setId).TermsById(&termId).Patch(requestBody)


```