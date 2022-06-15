---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 355e8f1c1c5f06b2a58363e0d4a46cc87f86175c
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098792"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationRubric()
displayName := "Example Credit Rubric"
requestBody.SetDisplayName(&displayName)
description := msgraphsdk.NewEducationItemBody()
requestBody.SetDescription(description)
content := "This is an example of a credit rubric (no points)"
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
    msgraphsdk.NewRubricLevel(),
displayName := "Poor"
    SetDisplayName(&displayName)
description := msgraphsdk.NewEducationItemBody()
    SetDescription(description)
content := ""
    description.SetContent(&content)
contentType := "text"
    description.SetContentType(&contentType)
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
}
result, err := graphClient.Education().Me().Rubrics().Post(requestBody)


```