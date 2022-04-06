---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d1825725f4648c40409136de5c86f54403fe4c8a
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757690"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "name": "My Day at the Beach",
    "@microsoft.graph.conflictBehavior": "rename",
    "children":  []Object {
    }
}
options := &msgraphsdk.BundlesRequestBuilderPostOptions{
    Body: requestBody,
}
graphClient.Drive().Bundles().Post(options)


```