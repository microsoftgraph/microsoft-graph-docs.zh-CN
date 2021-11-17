---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: abd159315886182518494339426b1e7d03747d3c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61031193"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.DevicesRequestBuilderGetQueryParameters{
    Search: "%22displayName:Android%22",
    Count: true,
}
headers := map[string]string{
    "ConsistencyLevel": "eventual"
}
options := &msgraphsdk.DevicesRequestBuilderGetOptions{
    Q: requestParameters,
    H: headers,
}
result, err := graphClient.Devices().Get(options)


```