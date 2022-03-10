---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: efcb080ca7ab1e3a82f7841d0feef016d8957f9e
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412416"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
tenantId := "String"
requestBody.SetTenantId(&tenantId)
tenantGroupId := "String"
requestBody.SetTenantGroupId(&tenantGroupId)
managementTemplateId := "String"
requestBody.SetManagementTemplateId(&managementTemplateId)
options := &msgraphsdk.ApplyRequestBuilderPostOptions{
    Body: requestBody,
}
managementActionId := "managementAction-id"
result, err := graphClient.TenantRelationships().ManagedTenants().ManagementActionsById(&managementActionId).Apply(managementAction-id).Post(options)


```