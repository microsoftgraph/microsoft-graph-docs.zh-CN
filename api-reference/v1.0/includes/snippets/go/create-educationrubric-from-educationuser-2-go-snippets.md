---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 683284b2b0eede66510d1424aaaebf482b6dba77
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325903"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationRubric()
displayName := "Example Points Rubric"
requestBody.SetDisplayName(&displayName)
description := msgraphsdk.NewEducationItemBody()
requestBody.SetDescription(description)
content := "This is an example of a rubric with points"
description.SetContent(&content)
contentType := "text"
description.SetContentType(&contentType)
requestBody.SetLevels( []RubricLevel {
    msgraphsdk.NewRubricLevel(),
    SetAdditionalData(map[string]interface{}{
        "displayName": "Good",
    }
    msgraphsdk.NewRubricLevel(),
    SetAdditionalData(map[string]interface{}{
        "displayName": "Poor",
    }
}
requestBody.SetQualities( []RubricQuality {
    msgraphsdk.NewRubricQuality(),
    SetAdditionalData(map[string]interface{}{
        "criteria":  []Object {
        }
        "weight": ,
    }
    msgraphsdk.NewRubricQuality(),
    SetAdditionalData(map[string]interface{}{
        "criteria":  []Object {
        }
        "weight": ,
    }
}
grading := msgraphsdk.NewEducationAssignmentGradeType()
requestBody.SetGrading(grading)
grading.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
}
result, err := graphClient.Education().Me().Rubrics().Post(requestBody)


```