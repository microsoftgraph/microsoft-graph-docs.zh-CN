---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a79d153f9e072576942ff294f77bd17773e2ae37
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61004219"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.UpdatableAssetsRequestBuilderGetQueryParameters{
    Filter: "isof('microsoft.graph.windowsUpdates.azureADDevice')",
}
options := &msgraphsdk.UpdatableAssetsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Admin().Windows().Updates().UpdatableAssets().Get(options)


```