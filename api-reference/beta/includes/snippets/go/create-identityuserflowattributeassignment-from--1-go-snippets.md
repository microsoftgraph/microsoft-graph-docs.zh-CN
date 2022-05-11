---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 87e882f1d94529456d4445c75aaf6ffb3a694f98
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326476"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewIdentityUserFlowAttributeAssignment()
isOptional := false
requestBody.SetIsOptional(&isOptional)
requiresVerification := false
requestBody.SetRequiresVerification(&requiresVerification)
userInputType := "TextBox"
requestBody.SetUserInputType(&userInputType)
displayName := "Shoe size"
requestBody.SetDisplayName(&displayName)
requestBody.SetUserAttributeValues( []UserAttributeValuesItem {
}
userAttribute := msgraphsdk.NewIdentityUserFlowAttribute()
requestBody.SetUserAttribute(userAttribute)
id := "extension_guid_shoeSize"
userAttribute.SetId(&id)
b2cIdentityUserFlowId := "b2cIdentityUserFlow-id"
result, err := graphClient.Identity().B2cUserFlowsById(&b2cIdentityUserFlowId).UserAttributeAssignments().Post(requestBody)


```