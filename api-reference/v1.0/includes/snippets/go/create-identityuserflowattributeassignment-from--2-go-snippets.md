---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 80e4d77476dc7c1114118d0698e55e687dc60a7d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082735"
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
userAttribute.SetAdditionalData(map[string]interface{}{
    "id": "extension_guid_shoeSize",
}
options := &msgraphsdk.UserAttributeAssignmentsRequestBuilderPostOptions{
    Body: requestBody,
}
b2xIdentityUserFlowId := "b2xIdentityUserFlow-id"
result, err := graphClient.Identity().B2xUserFlowsById(&b2xIdentityUserFlowId).UserAttributeAssignments().Post(options)


```