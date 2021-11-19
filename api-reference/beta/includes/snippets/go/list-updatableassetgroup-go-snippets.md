---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae503042a1ed87cf3a9e274410c3e0072b32e85e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083628"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UpdatableAssetsRequestBuilderGetQueryParameters{
    Filter: "isof('microsoft.graph.windowsUpdates.updatableAssetGroup')",
}
options := &msgraphsdk.UpdatableAssetsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Admin().Windows().Updates().UpdatableAssets().Get(options)


```