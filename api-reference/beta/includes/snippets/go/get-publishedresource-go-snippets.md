---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f8a235b8957343277195efdb7389b1aee56adb1
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100277"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.PublishedResourceRequestBuilderGetQueryParameters{
    Expand: "agentGroups",
}
options := &msgraphsdk.PublishedResourceRequestBuilderGetOptions{
    Q: requestParameters,
}
onPremisesPublishingProfileId := "onPremisesPublishingProfile-id"
publishedResourceId := "publishedResource-id"
result, err := graphClient.OnPremisesPublishingProfilesById(&onPremisesPublishingProfileId).PublishedResourcesById(&publishedResourceId).Get(options)


```