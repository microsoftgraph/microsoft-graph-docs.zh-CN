---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 62bd118471da0393995e43c255cd9441f5418865
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61024877"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
options := &msgraphsdk.RubricsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Education().Me().Rubrics().Post(options)


```