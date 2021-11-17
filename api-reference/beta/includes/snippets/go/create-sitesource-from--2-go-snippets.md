---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c736ddd08541255960ee62e78a4c8fe20f18f61a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60986746"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewSiteSource()
site := msgraphsdk.NewSite()
requestBody.SetSite(site)
webUrl := "https://contoso.sharepoint.com/sites/SecretSite"
site.SetWebUrl(&webUrl)
options := &msgraphsdk.SiteSourcesRequestBuilderPostOptions{
    Body: requestBody,
}
caseId := "case-id"
legalHoldId := "legalHold-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).LegalHoldsById(&legalHoldId).SiteSources().Post(options)


```