---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 376898c51376fc82a508a9dad1daeea16dd82d0e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092176"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPublishedResource()
displayName := "Demo provisioning (updated)"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.PublishedResourceRequestBuilderPatchOptions{
    Body: requestBody,
}
onPremisesPublishingProfileId := "onPremisesPublishingProfile-id"
publishedResourceId := "publishedResource-id"
graphClient.OnPremisesPublishingProfilesById(&onPremisesPublishingProfileId).PublishedResourcesById(&publishedResourceId).Patch(options)


```