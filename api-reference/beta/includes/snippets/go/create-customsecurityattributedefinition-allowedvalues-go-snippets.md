---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 18babb3b00e8bc3cc40a3cbfae4a6a153f33d637
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328442"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCustomSecurityAttributeDefinition()
attributeSet := "Engineering"
requestBody.SetAttributeSet(&attributeSet)
description := "Active projects for user"
requestBody.SetDescription(&description)
isCollection := true
requestBody.SetIsCollection(&isCollection)
isSearchable := true
requestBody.SetIsSearchable(&isSearchable)
name := "Project"
requestBody.SetName(&name)
status := "Available"
requestBody.SetStatus(&status)
type := "String"
requestBody.SetType(&type)
usePreDefinedValuesOnly := true
requestBody.SetUsePreDefinedValuesOnly(&usePreDefinedValuesOnly)
requestBody.SetAllowedValues( []AllowedValue {
    msgraphsdk.NewAllowedValue(),
    SetAdditionalData(map[string]interface{}{
        "id": "Alpine",
        "isActive": true,
    }
    msgraphsdk.NewAllowedValue(),
    SetAdditionalData(map[string]interface{}{
        "id": "Baker",
        "isActive": true,
    }
    msgraphsdk.NewAllowedValue(),
    SetAdditionalData(map[string]interface{}{
        "id": "Cascade",
        "isActive": true,
    }
}
result, err := graphClient.Directory().CustomSecurityAttributeDefinitions().Post(requestBody)


```