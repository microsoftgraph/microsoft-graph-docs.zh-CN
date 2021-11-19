---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 81b1fcaa3f85d4f65186c04411ab708d2a9e5e43
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098021"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.SubmissionsRequestBuilderGetQueryParameters{
    Expand: "outcomes",
}
options := &msgraphsdk.SubmissionsRequestBuilderGetOptions{
    Q: requestParameters,
}
educationClassId := "educationClass-id"
educationAssignmentId := "educationAssignment-id"
result, err := graphClient.Education().ClassesById(&educationClassId).AssignmentsById(&educationAssignmentId).Submissions().Get(options)


```