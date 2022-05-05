---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6880e5c6ecac42bdeda428e9c9139bf4cb40d082
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65206206"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.DirectoryObjectRequestBuilderGetQueryParameters{
    Count: true,
    OrderBy: "displayName",
    Filter: "startswith(displayName,%20'A')",
}
headers := map[string]string{
    "ConsistencyLevel": "eventual"
}
options := &msgraphsdk.DirectoryObjectRequestBuilderGetOptions{
    Q: requestParameters,
    H: headers,
}
deviceId := "device-id"
directoryObjectId := "directoryObject-id"
result, err := graphClient.DevicesById(&deviceId).MemberOfById(&directoryObjectId).Get(options)


```