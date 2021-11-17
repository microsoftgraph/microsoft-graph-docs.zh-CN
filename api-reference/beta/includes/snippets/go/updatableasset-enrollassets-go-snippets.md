---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 67280fccb5028d5f38977f74390ada3ad7e67fe6
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019255"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
updateCategory := "String"
requestBody.SetUpdateCategory(&updateCategory)
requestBody.SetAssets( []UpdatableAsset {
    msgraphsdk.NewUpdatableAsset(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
        "id": "String (identifier)",
    }
}
options := &msgraphsdk.EnrollAssetsRequestBuilderPostOptions{
    Body: requestBody,
}
graphClient.Admin().Windows().Updates().UpdatableAssets().EnrollAssets().Post(options)


```