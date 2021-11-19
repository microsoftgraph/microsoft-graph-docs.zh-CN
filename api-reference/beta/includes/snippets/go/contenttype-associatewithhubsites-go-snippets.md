---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 10aaa33bb1db2d2866751a3a645159a30da05976
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084310"
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
graphClient.SitesById(&siteId).ContentTypesById(&contentTypeId).AssociateWithHubSites().Post(options)


```