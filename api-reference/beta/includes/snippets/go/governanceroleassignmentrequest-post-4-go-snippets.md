---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e94eb3310225669d811a61eda536d63ff4b9cac5
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60990309"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewGovernanceRoleAssignmentRequest()
roleDefinitionId := "65bb4622-61f5-4f25-9d75-d0e20cf92019"
requestBody.SetRoleDefinitionId(&roleDefinitionId)
resourceId := "e5e7d29d-5465-45ac-885f-4716a5ee74b5"
requestBody.SetResourceId(&resourceId)
subjectId := "74765671-9ca4-40d7-9e36-2f4a570608a6"
requestBody.SetSubjectId(&subjectId)
assignmentState := "Eligible"
requestBody.SetAssignmentState(&assignmentState)
type := "AdminRemove"
requestBody.SetType(&type)
options := &msgraphsdk.RoleAssignmentRequestsRequestBuilderPostOptions{
    Body: requestBody,
}
privilegedAccessId := "privilegedAccess-id"
result, err := graphClient.PrivilegedAccessById(&privilegedAccessId).RoleAssignmentRequests().Post(options)


```