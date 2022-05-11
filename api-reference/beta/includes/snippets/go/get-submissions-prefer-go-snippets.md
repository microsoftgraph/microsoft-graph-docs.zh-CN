---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 31e151ed67452e5c58f4cdc11f1492493efeb82e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328373"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

headers := map[string]string{
    "Prefer": "include-unknown-enum-members"
}
options := &msgraphsdk.SubmissionsRequestBuilderGetRequestConfiguration{
    Headers: headers,
}
educationClassId := "educationClass-id"
educationAssignmentId := "educationAssignment-id"
result, err := graphClient.Education().ClassesById(&educationClassId).AssignmentsById(&educationAssignmentId).Submissions().GetWithRequestConfigurationAndResponseHandler(options, nil)


```