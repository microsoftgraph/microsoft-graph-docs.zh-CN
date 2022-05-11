---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 25b5acb5bc83705e369ad50496a304d1b1662b50
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328596"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPublishedResource()
displayName := "New provisioning"
requestBody.SetDisplayName(&displayName)
resourceName := "domain1.contoso.com"
requestBody.SetResourceName(&resourceName)
onPremisesPublishingProfileId := "onPremisesPublishingProfile-id"
result, err := graphClient.OnPremisesPublishingProfilesById(&onPremisesPublishingProfileId).PublishedResources().Post(requestBody)


```