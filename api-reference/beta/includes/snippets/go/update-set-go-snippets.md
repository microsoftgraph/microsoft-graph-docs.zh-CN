---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ffc90edc0ac00e33d25ec122f520a422d2d7fe2
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61017351"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewSet()
description := "mySet"
requestBody.SetDescription(&description)
options := &msgraphsdk.SetRequestBuilderPatchOptions{
    Body: requestBody,
}
setId := "set-id"
graphClient.TermStore().SetsById(&setId).Patch(options)


```