---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5cc230bb6e363111df6de4e2b06935ae52bbe96f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089373"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.MeRequestBuilderGetQueryParameters{
    Expand: "manager($levels=max;$select=id,displayName)",
    Select: "id,displayName",
    Count: true,
}
headers := map[string]string{
    "ConsistencyLevel": "eventual"
}
options := &msgraphsdk.MeRequestBuilderGetOptions{
    Q: requestParameters,
    H: headers,
}
result, err := graphClient.Me().Get(options)


```