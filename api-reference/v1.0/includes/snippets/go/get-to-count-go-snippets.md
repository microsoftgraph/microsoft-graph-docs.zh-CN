---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f4f959fe776054d1f715df4440d0661f19a44cb3
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62100789"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UsersRequestBuilderGetQueryParameters{
    Search: "%22displayName:wa%22%20OR%20%22displayName:ad%22",
    OrderbydisplayName: "",
    Count: true,
}
headers := map[string]string{
    "ConsistencyLevel": "eventual"
}
options := &msgraphsdk.UsersRequestBuilderGetOptions{
    Q: requestParameters,
    H: headers,
}
result, err := graphClient.Users().Get(options)


```