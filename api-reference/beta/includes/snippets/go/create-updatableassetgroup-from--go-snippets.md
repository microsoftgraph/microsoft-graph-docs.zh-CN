---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ffa50ce112c00ecf3de8b967b54b751620738d1
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327410"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUpdatableAsset()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetGroup",
}
result, err := graphClient.Admin().Windows().Updates().UpdatableAssets().Post(requestBody)


```