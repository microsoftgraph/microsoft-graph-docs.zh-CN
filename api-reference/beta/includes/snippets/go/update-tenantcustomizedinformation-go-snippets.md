---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cffabbcdc8166d8b0d33c3f6351a535e3545779c
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412756"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTenantCustomizedInformation()
tenantId := "String"
requestBody.SetTenantId(&tenantId)
requestBody.SetContacts( []TenantContactInformation {
    msgraphsdk.NewTenantContactInformation(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "microsoft.graph.managedTenants.tenantContactInformation",
        "name": "String",
        "title": "String",
        "email": "String",
        "phone": "String",
        "notes": "String",
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
result, err := graphClient.TenantRelationships().ManagedTenants().TenantsCustomizedInformationById(&tenantCustomizedInformationId).Patch(options)


```