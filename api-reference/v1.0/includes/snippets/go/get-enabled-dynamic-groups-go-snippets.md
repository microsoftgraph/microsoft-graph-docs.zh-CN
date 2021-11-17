---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 76e023c9f0d0980fb0f0948bf7d1116542c6c6ba
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60976592"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.GroupsRequestBuilderGetQueryParameters{
    Filter: "mailEnabled%20eq%20false%20and%20securityEnabled%20eq%20true%20and%20NOT(groupTypes/any(s:s%20eq%20'Unified'))%20and%20membershipRuleProcessingState%20eq%20'On'",
    Count: true,
    Select: "id,membershipRule,membershipRuleProcessingState",
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