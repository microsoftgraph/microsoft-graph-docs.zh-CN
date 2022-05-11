---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e1295919c082222da5ce2dcc35427e3789c7afba
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326740"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.MembersRequestBuilderGetQueryParameters{
    Filter: "(microsoft.graph.aadUserConversationMember/userId%20eq%20'73761f06-2ac9-469c-9f10-279a8cc267f9')",
}
options := &msgraphsdk.MembersRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Members().GetWithRequestConfigurationAndResponseHandler(options, nil)


```