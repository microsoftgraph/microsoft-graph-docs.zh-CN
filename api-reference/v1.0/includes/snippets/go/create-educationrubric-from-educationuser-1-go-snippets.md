---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cbe076a09333309d44e750218fa16f90bdbbaf4b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089981"
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
    }
    msgraphsdk.NewRubricQuality(),
    SetAdditionalData(map[string]interface{}{
        "criteria":  []Object {
        }
    }
}
options := &msgraphsdk.RubricsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Education().Me().Rubrics().Post(options)


```