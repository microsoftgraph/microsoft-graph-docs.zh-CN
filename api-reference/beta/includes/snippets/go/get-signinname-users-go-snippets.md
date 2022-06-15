---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 58cea2cadd5856747b2247dfd485dbb3f79e14c8
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095581"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UsersRequestBuilderGetQueryParameters{
    Select: "displayName,id",
    Filter: "identities/any(c:c/issuerAssignedId%20eq%20'j.smith@yahoo.com'%20and%20c/issuer%20eq%20'My%20B2C%20tenant')",
}
options := &msgraphsdk.UsersRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.Users().GetWithRequestConfigurationAndResponseHandler(options, nil)


```