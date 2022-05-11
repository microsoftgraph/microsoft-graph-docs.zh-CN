---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 37e49c51a17f833f5bf57dc59a231ff541e68a09
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325758"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.AppRoleAssignmentsRequestBuilderGetQueryParameters{
    Filter: "resourceId%20eq%208e881353-1735-45af-af21-ee1344582a4d",
}
options := &msgraphsdk.AppRoleAssignmentsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
userId := "user-id"
result, err := graphClient.UsersById(&userId).AppRoleAssignments().GetWithRequestConfigurationAndResponseHandler(options, nil)


```