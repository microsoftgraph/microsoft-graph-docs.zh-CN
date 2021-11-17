---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3762ed39a06c4c1a0bc66e222f1fe02b5710200a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60987249"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewClaimsMappingPolicy()
requestBody.SetDefinition( []String {
    "{"ClaimsMappingPolicy":{"Version":1,"IncludeBasicClaimSet":"true","ClaimsSchema": [{"Source":"user","ID":"userprincipalname","SamlClaimType":"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/nameidentifier"},{"Source":"user","ID":"givenname","SamlClaimType":"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/givenname"},{"Source":"user","ID":"displayname","SamlClaimType":"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/name"},{"Source":"user","ID":"surname","SamlClaimType":"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/surname"},{"Source":"user","ID":"userprincipalname","SamlClaimType":"username"}],"ClaimsTransformation":[{"ID":"CreateTermsOfService","TransformationMethod":"CreateStringClaim","InputParameters": [{"ID":"value","DataType":"string", "Value":"sandbox"}],"OutputClaims":[{"ClaimTypeReferenceId":"TOS","TransformationClaimType":"createdClaim"}]}]}}",
}
displayName := "Test1234"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.ClaimsMappingPoliciesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Policies().ClaimsMappingPolicies().Post(options)


```