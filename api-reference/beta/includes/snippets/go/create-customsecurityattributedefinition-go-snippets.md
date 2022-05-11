---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 48d97ddd5ab836ec59ca9bf00aff37f704f9d00f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328443"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCustomSecurityAttributeDefinition()
attributeSet := "Engineering"
requestBody.SetAttributeSet(&attributeSet)
description := "Target completion date"
requestBody.SetDescription(&description)
isCollection := false
requestBody.SetIsCollection(&isCollection)
isSearchable := true
requestBody.SetIsSearchable(&isSearchable)
name := "ProjectDate"
requestBody.SetName(&name)
status := "Available"
requestBody.SetStatus(&status)
type := "String"
requestBody.SetType(&type)
usePreDefinedValuesOnly := false
requestBody.SetUsePreDefinedValuesOnly(&usePreDefinedValuesOnly)
result, err := graphClient.Directory().CustomSecurityAttributeDefinitions().Post(requestBody)


```