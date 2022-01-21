---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b631a0d9cea2e52570014251ecc853aa5945790c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62098562"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewBaseTaskList()
displayName := "Shopping list"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.ListsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Tasks().Lists().Post(options)


```