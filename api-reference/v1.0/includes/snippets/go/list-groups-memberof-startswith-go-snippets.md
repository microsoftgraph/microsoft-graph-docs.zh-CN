---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c7dd8a7dff91d0dafded735a88724fff41d4307b
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209520"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.DirectoryObjectRequestBuilderGetQueryParameters{
    Count: true,
    Orderby: "displayName",
    Filter: "startswith(displayName,%20'A')",
}
headers := map[string]string{
    "ConsistencyLevel": "eventual"
}
options := &msgraphsdk.DirectoryObjectRequestBuilderGetOptions{
    Q: requestParameters,
    H: headers,
}
groupId := "group-id"
directoryObjectId := "directoryObject-id"
result, err := graphClient.GroupsById(&groupId).MemberOfById(&directoryObjectId).Get(options)


```