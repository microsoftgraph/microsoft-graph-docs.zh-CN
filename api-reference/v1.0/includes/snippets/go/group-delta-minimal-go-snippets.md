---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a55f0e949bc13d0b83f19f92aef8ae7277cf667
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61000105"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.GroupRequestBuilderGetQueryParameters{
    Select: "displayName,description,mailNickname",
}
headers := map[string]string{
    "Prefer": "return=minimal"
}
options := &msgraphsdk.GroupRequestBuilderGetOptions{
    Q: requestParameters,
    H: headers,
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).Get(options)


```