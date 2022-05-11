---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c3d6d801c2fa13b4abc3ed93a66e4936d32f9350
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327462"
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
educationClassId := "educationClass-id"
graphClient.Education().ClassesById(&educationClassId).AssignmentDefaults().Patch(requestBody)


```