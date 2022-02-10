---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8909113e1beeb5a8a75501b08b29e87f3fccf790
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519332"
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
options := &msgraphsdk.CustomSecurityAttributeDefinitionsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Directory().CustomSecurityAttributeDefinitions().Post(options)


```