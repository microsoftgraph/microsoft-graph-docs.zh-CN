---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f193217565d4fe511ffa9f0887aff184e899e8f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325773"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.SitesRequestBuilderGetQueryParameters{
    Select: "siteCollection,webUrl",
    Filter: "siteCollection/root%20ne%20null",
}
options := &msgraphsdk.SitesRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.Sites().GetWithRequestConfigurationAndResponseHandler(options, nil)


```