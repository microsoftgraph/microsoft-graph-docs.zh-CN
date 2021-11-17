---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6af649c1a3379f0479761907f36bd6df6070cab0
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61013628"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.UnifiedRoleAssignmentRequestBuilderGetQueryParameters{
    Expand: "roleDefinition,principal,directoryScope",
}
options := &msgraphsdk.UnifiedRoleAssignmentRequestBuilderGetOptions{
    Q: requestParameters,
}
unifiedRoleAssignmentId := "unifiedRoleAssignment-id"
result, err := graphClient.RoleManagement().Directory().RoleAssignmentsById(&unifiedRoleAssignmentId).Get(options)


```