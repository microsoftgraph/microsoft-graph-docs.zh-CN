---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef0b676acaa0861352f5a4256c4aa912338b16ca
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097769"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UnifiedRoleAssignmentRequestBuilderGetQueryParameters{
    Expand: "roleDefinition,principal,directoryScope",
}
options := &msgraphsdk.UnifiedRoleAssignmentRequestBuilderGetOptions{
    Q: requestParameters,
}
unifiedRoleAssignmentId := "unifiedRoleAssignment-id"
result, err := graphClient.RoleManagement().Directory().RoleAssignmentsById(&unifiedRoleAssignmentId).Get(options)


```