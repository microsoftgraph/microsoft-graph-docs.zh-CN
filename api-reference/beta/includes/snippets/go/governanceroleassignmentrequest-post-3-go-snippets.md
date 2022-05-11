---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 41db6448ce954eedacaa7fb4df3e88ba71d9b374
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328722"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewGovernanceRoleAssignmentRequest()
roleDefinitionId := "bc75b4e6-7403-4243-bf2f-d1f6990be122"
requestBody.SetRoleDefinitionId(&roleDefinitionId)
resourceId := "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735"
requestBody.SetResourceId(&resourceId)
subjectId := "918e54be-12c4-4f4c-a6d3-2ee0e3661c51"
requestBody.SetSubjectId(&subjectId)
assignmentState := "Active"
requestBody.SetAssignmentState(&assignmentState)
type := "UserRemove"
requestBody.SetType(&type)
reason := "Deactivate the role"
requestBody.SetReason(&reason)
linkedEligibleRoleAssignmentId := "cb8a533e-02d5-42ad-8499-916b1e4822ec"
requestBody.SetLinkedEligibleRoleAssignmentId(&linkedEligibleRoleAssignmentId)
privilegedAccessId := "privilegedAccess-id"
result, err := graphClient.PrivilegedAccessById(&privilegedAccessId).RoleAssignmentRequests().Post(requestBody)


```