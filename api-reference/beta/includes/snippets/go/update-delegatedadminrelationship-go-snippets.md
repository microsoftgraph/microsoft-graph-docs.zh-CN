---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6550e0fdd33a1fd76267e394826c4b667a9e647e
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203165"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDelegatedAdminRelationship()
displayName := "Updated Contoso admin relationship"
requestBody.SetDisplayName(&displayName)
duration := "P31D"
requestBody.SetDuration(&duration)
customer := msgraphsdk.NewDelegatedAdminRelationshipCustomerParticipant()
requestBody.SetCustomer(customer)
tenantId := "52eaad04-13a2-4a2f-9ce8-93a294fadf36"
customer.SetTenantId(&tenantId)
accessDetails := msgraphsdk.NewDelegatedAdminAccessDetails()
requestBody.SetAccessDetails(accessDetails)
accessDetails.SetUnifiedRoles( []UnifiedRole {
    msgraphsdk.NewUnifiedRole(),
    SetAdditionalData(map[string]interface{}{
        "roleDefinitionId": "44367163-eba1-44c3-98af-f5787879f96a",
    }
    msgraphsdk.NewUnifiedRole(),
    SetAdditionalData(map[string]interface{}{
        "roleDefinitionId": "29232cdf-9323-42fd-ade2-1d097af3e4de",
    }
    msgraphsdk.NewUnifiedRole(),
    SetAdditionalData(map[string]interface{}{
        "roleDefinitionId": "69091246-20e8-4a56-aa4d-066075b2a7a8",
    }
    msgraphsdk.NewUnifiedRole(),
    SetAdditionalData(map[string]interface{}{
        "roleDefinitionId": "3a2c62db-5318-420d-8d74-23affee5d9d5",
    }
}
headers := map[string]string{
    "If-Match": "W/"JyI0NzAwNjg0NS0wMDAwLTE5MDAtMDAwMC02MGY0Yjg4MzAwMDAiJw==""
}
options := &msgraphsdk.DelegatedAdminRelationshipRequestBuilderPatchOptions{
    Body: requestBody,
    H: headers,
}
delegatedAdminRelationshipId := "delegatedAdminRelationship-id"
graphClient.TenantRelationships().DelegatedAdminRelationshipsById(&delegatedAdminRelationshipId).Patch(options)


```