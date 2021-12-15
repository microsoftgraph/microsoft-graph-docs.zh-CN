---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e26044c53d7ce7e90ea2d2b19491eb94191f2820
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525844"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

headers := map[string]string{
    "Prefer": "include-unknown-enum-members"
}
options := &msgraphsdk.SubmissionsRequestBuilderGetOptions{
    H: headers,
}
educationClassId := "educationClass-id"
educationAssignmentId := "educationAssignment-id"
result, err := graphClient.Education().ClassesById(&educationClassId).AssignmentsById(&educationAssignmentId).Submissions().Get(options)


```