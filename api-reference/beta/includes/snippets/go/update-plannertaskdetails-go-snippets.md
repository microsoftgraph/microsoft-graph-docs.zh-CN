---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c434909a827bf4bb7518ef4b54131dc584d331a8
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61104133"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

headers := map[string]string{
    "Prefer": "return=representation"
    "If-Match": "W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=""
}
options := &msgraphsdk.DetailsRequestBuilderPatchOptions{
    H: headers,
}
plannerTaskId := "plannerTask-id"
graphClient.Planner().TasksById(&plannerTaskId).Details().Patch(options)


```