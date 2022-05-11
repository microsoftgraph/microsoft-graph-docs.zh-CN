---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c0bd90f854d48a15cd7d803649ef1123290d6c8
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328499"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ItemsRequestBuilderGetQueryParameters{
    Expand: "fields(select=Name,Color,Quantity)",
}
options := &msgraphsdk.ItemsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
siteId := "site-id"
listId := "list-id"
result, err := graphClient.SitesById(&siteId).ListsById(&listId).Items().GetWithRequestConfigurationAndResponseHandler(options, nil)


```