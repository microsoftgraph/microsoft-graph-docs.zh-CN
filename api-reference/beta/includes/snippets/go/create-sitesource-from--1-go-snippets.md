---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e28a02a93b32739206a14758f3aa8e6072c5f7a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60986956"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewSiteSource()
site := msgraphsdk.NewSite()
requestBody.SetSite(site)
webUrl := "https://contoso.sharepoint.com/sites/HumanResources"
site.SetWebUrl(&webUrl)
options := &msgraphsdk.SiteSourcesRequestBuilderPostOptions{
    Body: requestBody,
}
caseId := "case-id"
custodianId := "custodian-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).CustodiansById(&custodianId).SiteSources().Post(options)


```