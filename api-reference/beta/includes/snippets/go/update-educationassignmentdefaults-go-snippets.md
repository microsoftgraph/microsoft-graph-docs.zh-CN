---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d9759d36ef8b68271464e01c2e94a9105847efe
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412382"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationAssignmentDefaults()
addedStudentAction := "assignIfOpen"
requestBody.SetAddedStudentAction(&addedStudentAction)
addToCalendarAction := "studentsAndTeamOwners"
requestBody.SetAddToCalendarAction(&addToCalendarAction)
notificationChannelUrl := "https://graph.microsoft.com/beta/teams('id')/channels('id')"
requestBody.SetNotificationChannelUrl(&notificationChannelUrl)
options := &msgraphsdk.AssignmentDefaultsRequestBuilderPatchOptions{
    Body: requestBody,
}
educationClassId := "educationClass-id"
result, err := graphClient.Education().ClassesById(&educationClassId).AssignmentDefaults().Patch(options)


```