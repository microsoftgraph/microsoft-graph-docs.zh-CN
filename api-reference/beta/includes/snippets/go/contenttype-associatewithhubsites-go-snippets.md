---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5068cf1cb813dac91e98359225fa5c481bc07ce3
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411769"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetHubSiteUrls( []String {
    "https://graph.microsoft.com/beta/sites/id",
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