---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1762d786057164e1f47d26a80ccece8319b24eee
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088617"
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
b2cIdentityUserFlowId := "b2cIdentityUserFlow-id"
result, err := graphClient.Identity().B2cUserFlowsById(&b2cIdentityUserFlowId).UserAttributeAssignments().Post(options)


```