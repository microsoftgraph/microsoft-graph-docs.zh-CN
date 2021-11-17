---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 004c43b556994d2a3c327ace68f434a3b316db63
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61029917"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewUpdatableAsset()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetGroup",
}
options := &msgraphsdk.UpdatableAssetsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Admin().Windows().Updates().UpdatableAssets().Post(options)


```