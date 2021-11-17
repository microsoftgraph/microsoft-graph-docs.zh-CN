---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 82d50154688c44a547f33991df92aaba083ad28f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61006242"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewEducationAssignmentSettings()
submissionAnimationDisabled := true
requestBody.SetSubmissionAnimationDisabled(&submissionAnimationDisabled)
options := &msgraphsdk.AssignmentSettingsRequestBuilderPatchOptions{
    Body: requestBody,
}
educationClassId := "educationClass-id"
graphClient.Education().ClassesById(&educationClassId).AssignmentSettings().Patch(options)


```