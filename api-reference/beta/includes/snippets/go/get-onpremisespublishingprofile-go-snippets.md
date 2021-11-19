---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e3d3b39f5ee54d365ea5f57939ff25b050a659b9
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096066"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.OnPremisesPublishingProfileRequestBuilderGetQueryParameters{
    Expand: "publishedResources,agents,agentGroups",
}
options := &msgraphsdk.OnPremisesPublishingProfileRequestBuilderGetOptions{
    Q: requestParameters,
}
onPremisesPublishingProfileId := "onPremisesPublishingProfile-id"
result, err := graphClient.OnPremisesPublishingProfilesById(&onPremisesPublishingProfileId).Get(options)


```