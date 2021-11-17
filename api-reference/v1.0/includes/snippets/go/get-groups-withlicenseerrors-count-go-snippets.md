---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c63ebced0af46340af7bcdac48ba81ebc167509
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60976591"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.GroupsRequestBuilderGetQueryParameters{
    Count: true,
    Filter: "hasMembersWithLicenseErrors%20eq%20true",
    Select: "id,displayName",
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