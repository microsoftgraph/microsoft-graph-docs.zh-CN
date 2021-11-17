---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72c99a1bc75efd956ab04abd6249ce9828738fb4
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61016101"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.MembersRequestBuilderGetQueryParameters{
    Filter: "(microsoft.graph.aadUserConversationMember/displayName%20eq%20'Harry%20Johnson'%20or%20microsoft.graph.aadUserConversationMember/email%20eq%20'admin@M365x987948.OnMicrosoft.com')",
}
options := &msgraphsdk.MembersRequestBuilderGetOptions{
    Q: requestParameters,
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Members().Get(options)


```