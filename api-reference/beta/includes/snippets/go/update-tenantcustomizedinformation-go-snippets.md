---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06ce35b21f1f0273dacd5a4b4bbb40974aa3729b
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098785"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTenantCustomizedInformation()
tenantId := "String"
requestBody.SetTenantId(&tenantId)
requestBody.SetContacts( []TenantContactInformation {
    msgraphsdk.NewTenantContactInformation(),
name := "String"
    SetName(&name)
title := "String"
    SetTitle(&title)
email := "String"
    SetEmail(&email)
phone := "String"
    SetPhone(&phone)
notes := "String"
    SetNotes(&notes)
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "microsoft.graph.managedTenants.tenantContactInformation",
    }
}
website := "String"
requestBody.SetWebsite(&website)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.managedTenants.tenantCustomizedInformation",
}
tenantCustomizedInformationId := "tenantCustomizedInformation-id"
graphClient.TenantRelationships().ManagedTenants().TenantsCustomizedInformationById(&tenantCustomizedInformationId).Patch(requestBody)


```