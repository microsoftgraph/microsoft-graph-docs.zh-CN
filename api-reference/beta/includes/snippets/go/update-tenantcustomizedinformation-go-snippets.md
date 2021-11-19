---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 786a2c638b05991656e278212593c73961a75660
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098694"
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