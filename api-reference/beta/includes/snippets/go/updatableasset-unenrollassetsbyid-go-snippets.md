---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 861b97c372a4fd9be2dd7ba492b2d1206be9e7ed
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084357"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
updateCategory := "feature"
requestBody.SetUpdateCategory(&updateCategory)
memberEntityType := "#microsoft.graph.windowsUpdates.azureADDevice"
requestBody.SetMemberEntityType(&memberEntityType)
requestBody.SetIds( []String {
    "String",
    "String",
    "String",
}
options := &msgraphsdk.UnenrollAssetsByIdRequestBuilderPostOptions{
    Body: requestBody,
}
graphClient.Admin().Windows().Updates().UpdatableAssets().UnenrollAssetsById().Post(options)


```