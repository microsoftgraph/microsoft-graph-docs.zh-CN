---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c7d64febcd0d8508f817b96aa40ce620799bdb8
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65206541"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.MembersRequestBuilderGetQueryParameters{
    Count: true,
    Filter: "startswith(displayName,%20'a')",
}
headers := map[string]string{
    "ConsistencyLevel": "eventual"
}
options := &msgraphsdk.MembersRequestBuilderGetOptions{
    Q: requestParameters,
    H: headers,
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).Members().Get(options)


```