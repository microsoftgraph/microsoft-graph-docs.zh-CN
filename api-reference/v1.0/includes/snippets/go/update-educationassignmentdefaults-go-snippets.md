---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09ade5025bc47cf1f04bbf92f8b74d1e6995c021
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092260"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationAssignmentDefaults()
addedStudentAction := "assignIfOpen"
requestBody.SetAddedStudentAction(&addedStudentAction)
notificationChannelUrl := "https://graph.microsoft.com/beta/teams('acdefc6b-2dc6-4e71-b1e9-6d9810ab1793')/channels('3da03fc4-8eac-4459-84fb-1422dc01f65e')"
requestBody.SetNotificationChannelUrl(&notificationChannelUrl)
options := &msgraphsdk.AssignmentDefaultsRequestBuilderPatchOptions{
    Body: requestBody,
}
educationClassId := "educationClass-id"
graphClient.Education().ClassesById(&educationClassId).AssignmentDefaults().Patch(options)


```