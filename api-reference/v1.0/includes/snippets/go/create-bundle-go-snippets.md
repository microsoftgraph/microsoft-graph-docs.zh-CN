---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f7d2408057e9ccf8a76a0d94c9bf7a9a6db191a9
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328212"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "name": "Just some files",
    "@microsoft.graph.conflictBehavior": "rename",
    "children":  []Object {
    }
}
graphClient.Drive().Bundles().Post(requestBody)


```