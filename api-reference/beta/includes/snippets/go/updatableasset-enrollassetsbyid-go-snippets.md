---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ac768a5cac2faa1fbcaa4debe876452a4fd4258f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61101451"
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
options := &msgraphsdk.EnrollAssetsByIdRequestBuilderPostOptions{
    Body: requestBody,
}
graphClient.Admin().Windows().Updates().UpdatableAssets().EnrollAssetsById().Post(options)


```