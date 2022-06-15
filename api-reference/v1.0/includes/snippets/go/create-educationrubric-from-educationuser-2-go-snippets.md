---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4772ae2b832d5ea3c08d4fd3fc9811c1f7b31ce4
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098721"
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
displayName := "Good"
    SetDisplayName(&displayName)
description := msgraphsdk.NewEducationItemBody()
    SetDescription(description)
content := ""
    description.SetContent(&content)
contentType := "text"
    description.SetContentType(&contentType)
grading := msgraphsdk.NewEducationAssignmentGradeType()
    SetGrading(grading)
    grading.SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
        "maxPoints": ,
    }
    msgraphsdk.NewRubricLevel(),
displayName := "Poor"
    SetDisplayName(&displayName)
description := msgraphsdk.NewEducationItemBody()
    SetDescription(description)
content := ""
    description.SetContent(&content)
contentType := "text"
    description.SetContentType(&contentType)
grading := msgraphsdk.NewEducationAssignmentGradeType()
    SetGrading(grading)
    grading.SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
        "maxPoints": ,
    }
}
requestBody.SetQualities( []RubricQuality {
    msgraphsdk.NewRubricQuality(),
description := msgraphsdk.NewEducationItemBody()
    SetDescription(description)
content := "Argument"
    description.SetContent(&content)
contentType := "text"
    description.SetContentType(&contentType)
    SetCriteria( []RubricCriterion {
        msgraphsdk.NewRubricCriterion(),
description := msgraphsdk.NewEducationItemBody()
        SetDescription(description)
content := "The essay's argument is persuasive."
        description.SetContent(&content)
contentType := "text"
        description.SetContentType(&contentType)
        msgraphsdk.NewRubricCriterion(),
description := msgraphsdk.NewEducationItemBody()
        SetDescription(description)
content := "The essay's argument does not make sense."
        description.SetContent(&content)
contentType := "text"
        description.SetContentType(&contentType)
    }
weight := float32(50.0)
    SetWeight(&weight)
    msgraphsdk.NewRubricQuality(),
description := msgraphsdk.NewEducationItemBody()
    SetDescription(description)
content := "Spelling and Grammar"
    description.SetContent(&content)
contentType := "text"
    description.SetContentType(&contentType)
    SetCriteria( []RubricCriterion {
        msgraphsdk.NewRubricCriterion(),
description := msgraphsdk.NewEducationItemBody()
        SetDescription(description)
content := "The essay uses proper spelling and grammar with few or no errors."
        description.SetContent(&content)
contentType := "text"
        description.SetContentType(&contentType)
        msgraphsdk.NewRubricCriterion(),
description := msgraphsdk.NewEducationItemBody()
        SetDescription(description)
content := "The essay has numerous errors in spelling and/or grammar."
        description.SetContent(&content)
contentType := "text"
        description.SetContentType(&contentType)
    }
weight := float32(50.0)
    SetWeight(&weight)
}
grading := msgraphsdk.NewEducationAssignmentGradeType()
requestBody.SetGrading(grading)
grading.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
}
result, err := graphClient.Education().Me().Rubrics().Post(requestBody)


```