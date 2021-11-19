---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5707d9646de1b58fe2d0a2976b30fe4edeae6765
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085857"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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