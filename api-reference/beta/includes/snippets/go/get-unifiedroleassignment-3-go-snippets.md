---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 401d8ddb1af1a7dcc2304044616bcc0a993ba474
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61094978"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UnifiedRoleAssignmentMultipleRequestBuilderGetQueryParameters{
    Expand: "roleDefinition",
}
options := &msgraphsdk.UnifiedRoleAssignmentMultipleRequestBuilderGetOptions{
    Q: requestParameters,
}
unifiedRoleAssignmentMultipleId := "unifiedRoleAssignmentMultiple-id"
result, err := graphClient.RoleManagement().CloudPC().RoleAssignmentsById(&unifiedRoleAssignmentMultipleId).Get(options)


```