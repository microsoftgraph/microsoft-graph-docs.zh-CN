---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 221725c44fb32b6dc857264a4f29fe4acb574002
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086143"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ApplicationsRequestBuilderGetQueryParameters{
    Search: "%22displayName:Web%22",
    Count: true,
}
headers := map[string]string{
    "ConsistencyLevel": "eventual"
}
options := &msgraphsdk.ApplicationsRequestBuilderGetOptions{
    Q: requestParameters,
    H: headers,
}
result, err := graphClient.Applications().Get(options)


```