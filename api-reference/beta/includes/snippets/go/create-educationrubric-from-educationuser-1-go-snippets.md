---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a452591c97cdadb60c15d1de0e144773eeb3c4f8
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61024878"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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