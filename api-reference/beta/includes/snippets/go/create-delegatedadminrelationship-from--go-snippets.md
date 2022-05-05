---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e25e2cb072995c8aaebe0774d8163f051e628e6e
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205430"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDelegatedAdminRelationship()
displayName := "Contoso admin relationship"
requestBody.SetDisplayName(&displayName)
duration := "P730D"
requestBody.SetDuration(&duration)
customer := msgraphsdk.NewDelegatedAdminRelationshipCustomerParticipant()
requestBody.SetCustomer(customer)
tenantId := "4b827261-d21f-4aa9-b7db-7fa1f56fb163"
customer.SetTenantId(&tenantId)
displayName := "Contoso subsidiary Inc"
customer.SetDisplayName(&displayName)
accessDetails := msgraphsdk.NewDelegatedAdminAccessDetails()
requestBody.SetAccessDetails(accessDetails)
accessDetails.SetUnifiedRoles( []UnifiedRole {
    msgraphsdk.NewUnifiedRole(),
    SetAdditionalData(map[string]interface{}{
        "roleDefinitionId": "29232cdf-9323-42fd-ade2-1d097af3e4de",
    }
    msgraphsdk.NewUnifiedRole(),
    SetAdditionalData(map[string]interface{}{
        "roleDefinitionId": "3a2c62db-5318-420d-8d74-23affee5d9d5",
    }
}
options := &msgraphsdk.DelegatedAdminRelationshipsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.TenantRelationships().DelegatedAdminRelationships().Post(options)


```