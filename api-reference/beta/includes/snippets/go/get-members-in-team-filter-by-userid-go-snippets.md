---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1eebd23ad388820082961be987acf0faf2b0656d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085561"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.MembersRequestBuilderGetQueryParameters{
    Filter: "(microsoft.graph.aadUserConversationMember/userId%20eq%20'73761f06-2ac9-469c-9f10-279a8cc267f9')",
}
options := &msgraphsdk.MembersRequestBuilderGetOptions{
    Q: requestParameters,
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Members().Get(options)


```