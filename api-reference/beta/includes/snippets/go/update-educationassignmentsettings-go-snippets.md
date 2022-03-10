---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88e3b891a8c2cb0a40fb14ca8e9912f40de5e63a
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412261"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationAssignmentSettings()
submissionAnimationDisabled := true
requestBody.SetSubmissionAnimationDisabled(&submissionAnimationDisabled)
options := &msgraphsdk.AssignmentSettingsRequestBuilderPatchOptions{
    Body: requestBody,
}
educationClassId := "educationClass-id"
result, err := graphClient.Education().ClassesById(&educationClassId).AssignmentSettings().Patch(options)


```