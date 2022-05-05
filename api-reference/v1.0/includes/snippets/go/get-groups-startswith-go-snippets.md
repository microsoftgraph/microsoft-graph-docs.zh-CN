---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ac71f981de7b05359f891d1fa6b0a1b1b01ed833
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209985"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.GroupsRequestBuilderGetQueryParameters{
    Filter: "startswith(displayName,%20'a')",
    Count: true,
    Top: 1,
    Orderby: "displayName",
}
headers := map[string]string{
    "ConsistencyLevel": "eventual"
}
options := &msgraphsdk.GroupsRequestBuilderGetOptions{
    Q: requestParameters,
    H: headers,
}
result, err := graphClient.Groups().Get(options)


```