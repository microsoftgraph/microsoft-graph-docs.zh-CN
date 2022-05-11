---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a8c6a64284b874d3ca73c8d0bf78057518d846ee
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328829"
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
result, err := graphClient.TenantRelationships().DelegatedAdminRelationships().Post(requestBody)


```