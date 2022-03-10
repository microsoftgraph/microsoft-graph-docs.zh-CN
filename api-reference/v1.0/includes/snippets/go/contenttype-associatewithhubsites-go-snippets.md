---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e9da542fefd721da5165a66acafb817f080834cf
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412703"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetHubSiteUrls( []String {
    "https://graph.microsoft.com/v1.0/sites/{site-id}",
}
propagateToExistingLists := false
requestBody.SetPropagateToExistingLists(&propagateToExistingLists)
options := &msgraphsdk.AssociateWithHubSitesRequestBuilderPostOptions{
    Body: requestBody,
}
siteId := "site-id"
contentTypeId := "contentType-id"
graphClient.SitesById(&siteId).ContentTypesById(&contentTypeId).AssociateWithHubSites(site-id, contentType-id).Post(options)


```