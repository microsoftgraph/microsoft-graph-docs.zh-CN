---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c82dae83803ae120ed9ee44fba80087ffb92851b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102369"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUpdatableAsset()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetGroup",
}
options := &msgraphsdk.UpdatableAssetsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Admin().Windows().Updates().UpdatableAssets().Post(options)


```