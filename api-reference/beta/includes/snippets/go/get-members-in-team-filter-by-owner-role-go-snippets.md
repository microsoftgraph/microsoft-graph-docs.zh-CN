---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a117b0054d13da8cb35d7721250e373fa71705f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327003"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.MembersRequestBuilderGetQueryParameters{
    Filter: "roles/any(r:r%20eq%20'owner')",
}
options := &msgraphsdk.MembersRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Members().GetWithRequestConfigurationAndResponseHandler(options, nil)


```