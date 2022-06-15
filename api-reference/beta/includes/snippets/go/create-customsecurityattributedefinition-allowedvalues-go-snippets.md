---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c1aba8fef9c8d6224b0bb06177c524488e97112
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098787"
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
id := "Alpine"
    SetId(&id)
isActive := true
    SetIsActive(&isActive)
    msgraphsdk.NewAllowedValue(),
id := "Baker"
    SetId(&id)
isActive := true
    SetIsActive(&isActive)
    msgraphsdk.NewAllowedValue(),
id := "Cascade"
    SetId(&id)
isActive := true
    SetIsActive(&isActive)
}
result, err := graphClient.Directory().CustomSecurityAttributeDefinitions().Post(requestBody)


```