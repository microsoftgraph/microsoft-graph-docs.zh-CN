---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 95f499c158e43cd012fd2b6338644bda4f18f3d8
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61016100"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.MembersRequestBuilderGetQueryParameters{
    Filter: "(microsoft.graph.aadUserConversationMember/userId%20eq%20'73761f06-2ac9-469c-9f10-279a8cc267f9')",
}
options := &msgraphsdk.MembersRequestBuilderGetOptions{
    Q: requestParameters,
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Members().Get(options)


```