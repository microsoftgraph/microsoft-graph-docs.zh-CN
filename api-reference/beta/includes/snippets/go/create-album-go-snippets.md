---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 031583d4f301fa22a2d80546959c601243ef47ef
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325947"
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
graphClient.Drive().Bundles().Post(requestBody)


```