---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8934d82cf746a74f8af6a08ba430a6a278934d88
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65314303"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.PrivilegedRoleAssignmentsRequestBuilderGetQueryParameters{
    Filter: "isElevated%20eq%20true%20and%20expirationDateTime%20eq%20null",
}
options := &msgraphsdk.PrivilegedRoleAssignmentsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.PrivilegedRoleAssignments().GetWithRequestConfigurationAndResponseHandler(options, nil)


```