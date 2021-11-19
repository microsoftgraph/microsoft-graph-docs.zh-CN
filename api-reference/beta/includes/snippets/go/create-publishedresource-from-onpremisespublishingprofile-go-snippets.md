---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d99235d801b2d436ace35af7b2404aba33cf3c92
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61094219"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPublishedResource()
displayName := "New provisioning"
requestBody.SetDisplayName(&displayName)
resourceName := "domain1.contoso.com"
requestBody.SetResourceName(&resourceName)
options := &msgraphsdk.PublishedResourcesRequestBuilderPostOptions{
    Body: requestBody,
}
onPremisesPublishingProfileId := "onPremisesPublishingProfile-id"
result, err := graphClient.OnPremisesPublishingProfilesById(&onPremisesPublishingProfileId).PublishedResources().Post(options)


```