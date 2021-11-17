---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 306009c8dd020807516681e042138f04f8742d23
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61011834"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewTenantCustomizedInformation()
tenantId := "String"
requestBody.SetTenantId(&tenantId)
requestBody.SetContacts( []TenantContactInformation {
    msgraphsdk.NewTenantContactInformation(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "microsoft.graph.managedTenants.tenantContactInformation",
    }
}
website := "String"
requestBody.SetWebsite(&website)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.managedTenants.tenantCustomizedInformation",
}
options := &msgraphsdk.TenantCustomizedInformationRequestBuilderPatchOptions{
    Body: requestBody,
}
tenantCustomizedInformationId := "tenantCustomizedInformation-id"
graphClient.TenantRelationships().ManagedTenants().TenantsCustomizedInformationById(&tenantCustomizedInformationId).Patch(options)


```