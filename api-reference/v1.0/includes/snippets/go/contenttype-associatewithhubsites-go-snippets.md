---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de878cd24d0992d9ce2b36e5b3f4623e9c77784f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326353"
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
siteId := "site-id"
contentTypeId := "contentType-id"
graphClient.SitesById(&siteId).ContentTypesById(&contentTypeId).AssociateWithHubSites(site-id, contentType-id).Post(requestBody)


```