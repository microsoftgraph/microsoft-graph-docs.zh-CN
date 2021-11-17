---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea4fec2463c5acd02df8801f753a6fc7e0404852
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60980947"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
result, err := graphClient.TenantRelationships().ManagedTenants().ManagementActionsById(&managementActionId).Apply().Post(options)


```