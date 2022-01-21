---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 402267c9a9abbc4ad5808067ecf79c1b0ce7b2c6
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62130452"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.EducationSubmissionRequestBuilderGetQueryParameters{
    Expand: "*",
}
options := &msgraphsdk.EducationSubmissionRequestBuilderGetOptions{
    Q: requestParameters,
}
educationClassId := "educationClass-id"
educationAssignmentId := "educationAssignment-id"
educationSubmissionId := "educationSubmission-id"
result, err := graphClient.Education().ClassesById(&educationClassId).AssignmentsById(&educationAssignmentId).SubmissionsById(&educationSubmissionId).Get(options)


```