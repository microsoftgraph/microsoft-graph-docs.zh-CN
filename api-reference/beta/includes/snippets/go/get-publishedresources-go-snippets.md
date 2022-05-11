---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 12ceb1bc8288814d8553c7ae6ddf01f891588212
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328147"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.PublishedResourcesRequestBuilderGetQueryParameters{
    Expand: "agentGroups",
}
options := &msgraphsdk.PublishedResourcesRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
onPremisesPublishingProfileId := "onPremisesPublishingProfile-id"
result, err := graphClient.OnPremisesPublishingProfilesById(&onPremisesPublishingProfileId).PublishedResources().GetWithRequestConfigurationAndResponseHandler(options, nil)


```