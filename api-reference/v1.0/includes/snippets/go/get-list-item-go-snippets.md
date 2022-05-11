---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3eb0d9f14b16129badcaadbab409cf448db0f469
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325813"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ListItemRequestBuilderGetQueryParameters{
    Expand: "fields",
}
options := &msgraphsdk.ListItemRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
siteId := "site-id"
listId := "list-id"
listItemId := "listItem-id"
result, err := graphClient.SitesById(&siteId).ListsById(&listId).ItemsById(&listItemId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```