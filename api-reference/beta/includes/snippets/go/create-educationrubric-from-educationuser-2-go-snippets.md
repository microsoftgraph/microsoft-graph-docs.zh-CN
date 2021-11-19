---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cafae7414c3b086ad4710f9a4724146fafdc10b7
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61104147"
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
options := &msgraphsdk.RubricsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Education().Me().Rubrics().Post(options)


```