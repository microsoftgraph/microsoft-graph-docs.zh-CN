---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 82d2ef7f9de25ccb6d780dda7e813fea2595f2d0
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61017214"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.UnifiedRoleAssignmentMultipleRequestBuilderGetQueryParameters{
    Expand: "roleDefinition",
}
options := &msgraphsdk.UnifiedRoleAssignmentMultipleRequestBuilderGetOptions{
    Q: requestParameters,
}
unifiedRoleAssignmentMultipleId := "unifiedRoleAssignmentMultiple-id"
result, err := graphClient.RoleManagement().CloudPC().RoleAssignmentsById(&unifiedRoleAssignmentMultipleId).Get(options)


```