---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 79d0900ae8089a8f611da31493ce61eb9000c1fd
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328136"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.TeamsRequestBuilderGetQueryParameters{
    Filter: "displayName%20eq%20'A%20Contoso%20Team'",
    Select: "id,description",
}
options := &msgraphsdk.TeamsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.Teams().GetWithRequestConfigurationAndResponseHandler(options, nil)


```